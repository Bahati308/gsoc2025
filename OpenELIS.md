# Improving E2E QA Tests
Some projects are assignments. Others are adventures. My Google Summer of Code journey was the latter—a deep dive into real-world problem-solving, open-source collaboration, and shipping features that actually matter.

Over the course of GSoC, I worked on Improving E2E QA Tests—an initiative to boost test coverage for our new React frontend from roughly 30% to over 80%. The mission was clear: close testing gaps, validate the entire application workflow, and integrate robust test suites into the CI/CD pipeline. This wasn’t just about adding tests—it was about building confidence in every deploy, protecting critical user flows, and elevating system reliability to production-grade standards.

What follows is not just a technical log, but the story of how an idea went from proposal to production—complete with hurdles, breakthroughs, and lessons that will outlast the program itself.

## Future Plans

## Merged Pull Request Links

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2208 - Dictionary fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2206 - Test Management E2E
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2202 - Test Notification Config
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2183 - BatchTest Reassignment And Cancelation-E2E
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2164 - Result Reporting Configuration E2E
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2140 - feat: Notify User-E2E
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2134 - Fix: Dictionary and User Management
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2104 - Dictionary-fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2103 - Dictionary-Fix
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
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1944 - E2E Hardening
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1887 - Revert "Updated breadcrumbs for Report"
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1847 - QA test-fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1824 - Workflow fix - changing to chrome
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1819 - result e2e fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1810 - Fix: minor dictionary issue
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1809 - fix: extra validation for result
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1807 - fix: test date validation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1806 - fix: menu translation issue
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1805 - fix: batch cancelation bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1784 - fix: QA menu fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1782 - fix: batch test assignment
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1771 - fix: QA organization menu fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1764 - fix: batch test reassignment validation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1759 - fix: barcode validation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1756 - fix: user management QA fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1750 - fix: menu config translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1748 - fix: organization management QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1745 - fix: provider management QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1743 - fix: barcode e2e
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1741 - fix: result reporting configuration
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1740 - fix: reflex test QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1739 - fix: batch test e2e
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1738 - fix: menu QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1737 - fix: barcode page bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1736 - fix: configuration translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1735 - fix: QA menu bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1734 - fix: test config translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1733 - fix: provider QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1732 - fix: dictionary menu bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1731 - fix: user management translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1729 - fix: barcode QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1727 - fix: user management e2e
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1726 - fix: barcode translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1725 - fix: organization e2e
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1724 - fix: provider e2e
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1723 - fix: QA dictionary
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1722 - fix: test name QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1721 - fix: menu QA bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1720 - fix: dictionary config translation
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1719 - fix: barcode config QA
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1718 - fix: QA bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1717 - fix: translation bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1716 - fix: dictionary menu config bug
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/1715 - fix: barcode translation bug

## Not Yet Merged.

https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2208 - Dictionary fix
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2206 - Test Management E2E
https://github.com/DIGI-UW/OpenELIS-Global-2/pull/2202 - Test Notification Config
