# Improving E2E QA Tests
Some projects are assignments. Others are adventures. My Google Summer of Code journey was the latter—a deep dive into real-world problem-solving, open-source collaboration, and shipping features that actually matter.

Over the course of GSoC, I worked on Improving E2E QA Tests—an initiative to boost test coverage for our new React frontend from roughly 30% to over 80%. The mission was clear: close testing gaps, validate the entire application workflow, and integrate robust test suites into the CI/CD pipeline. This wasn’t just about adding tests—it was about building confidence in every deploy, protecting critical user flows, and elevating system reliability to production-grade standards.

What follows is not just a technical log, but the story of how an idea went from proposal to production—complete with hurdles, breakthroughs, and lessons that will outlast the program itself.

## Identify gaps in the current E2E test suite.
The first step was understanding what wasn’t covered. Existing tests primarily validated surface-level interactions, leaving several edge cases and multi-step user journeys unchecked. For example, account recovery workflows, error-handling during network failures, and cross-browser behavior had little to no coverage. To tackle this, I conducted a systematic audit of the testing framework, cross-referencing user stories and production bugs against existing tests. This approach revealed clear blind spots and allowed us to prioritize critical areas that had the highest impact on user experience.

## Develop and implement additional E2E test cases to achieve the desired coverage.

Develop and implement additional E2E test cases to achieve the desired coverage

With the gaps identified, the next task was writing robust test cases to expand coverage. The focus wasn’t only on quantity, but on writing meaningful tests that simulated real-world user behavior. I introduced new test suites for login flows, data persistence, error boundaries, and permissions management. Each new test was designed to be modular, maintainable, and easy for future contributors to extend. By the end of the cycle, the project had moved from ~30% coverage to over 80%, ensuring that nearly all critical workflows were consistently validated.

## Optimize the test execution process to ensure efficiency and scalability

As the number of test cases grew, execution time became a bottleneck. Running all tests sequentially slowed down developer feedback, which could discourage consistent usage. To address this, I optimized the testing process by:

Enabling parallel test execution to reduce runtime.

Categorizing tests into smoke tests, regression tests, and full workflows, allowing teams to run the right set at the right time.

Investigating and fixing flaky tests, which often gave false negatives due to timing issues or unstable selectors.

This optimization ensured the test suite could scale with future growth while staying efficient.

### Example of a flaky selector

  ``` 
  // Using a CSS class that frequently changes

  cy.get('.btn-primary').click();
```
Problem: .btn-primary may change if the design changes, or there may be multiple buttons with that class.
 
Stable Version using data-cy:
```
cy.get('[data-cy="submit-button"]').click();
```
## Integrate E2E tests into the CI/CD pipeline for automated validation

A strong test suite is only valuable if it’s consistently used. To ensure long-term impact, I worked on integrating E2E tests directly into the CI/CD pipeline. Now, every pull request triggers automated test runs, blocking merges if critical workflows fail. This setup enforces a high standard of code quality, prevents regressions from slipping into production, and fosters confidence in continuous deployment. The integration also provides clear reporting for developers, helping them debug issues faster.

## Provide documentation and knowledge sharing to maintain test coverage over time

One of the biggest risks for any test suite is neglect over time. To prevent this, I created contributor-friendly documentation covering how to write new test cases, how to run tests locally, and how to interpret CI/CD test reports. I also shared best practices with the team through knowledge-transfer sessions, ensuring that future contributors can maintain and expand the test suite without friction. This step was essential for making the work sustainable beyond the GSoC program.

## Future Plans

The GSoC project delivered a stronger and more reliable testing framework, but there are opportunities to take this further. Looking ahead, the following plans will guide continued development:

Expand test coverage further by addressing advanced workflows such as integrations with third-party APIs, mobile responsiveness, and accessibility testing.

Introduce visual regression testing to catch unexpected UI changes that break design consistency.

Enhance CI/CD integration by adding test result dashboards and alerting mechanisms for failed builds.

Explore performance testing integration to ensure not only functional reliability but also speed and scalability under load.

Continue community training and mentorship, ensuring that knowledge about writing and maintaining tests spreads across contributors and doesn’t remain siloed.

## Merged Pull Request Links

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2183 - BatchTest Reassignment And Cancelation-E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2164 - Result Reporting Configuration E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2140 - feat: Notify User-E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2134 - Fix: Dictionary and User Management

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2104 - Dictionary-fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2085 - General Configurations-E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2075 - Fix: QA fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2070 - Provider Management E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2062 - Organization Management E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2057 - Menu Configuration-E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2053 - Fix: Dictionary Menu Fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2052 - Feat: Reflex Tests Configuration E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2049 - Barcode-E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2040 - Dictionary Menu E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2013 - feat: User Management E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2006 - fix: Result Test Hardening

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2005 - fix: Test Name Fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1992 - Fix:Login and Result fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1990 - FIX: Result fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1984 - Added validation by date

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1968 - Modified Result E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1954 - Nonconform E2E fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1949 - QA troubleshoot

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1887 - Revert "Updated breadcrumbs for Report"

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1847 - QA test-fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1824 - Workflow fix - changing to chrome

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1819 - result e2e fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1750 - fix: menu config translation

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1737 - fix: barcode page bug

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1734 - fix: test config translation

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1732 - fix: dictionary menu bug

## Not Yet Merged.

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2208 - Dictionary fix

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2206 - Test Management E2E

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2202 - Test Notification Config

### This GSoC project turned testing into trust—transforming gaps into coverage, code into confidence, and every deploy into a promise of reliability for both users and contributors.
