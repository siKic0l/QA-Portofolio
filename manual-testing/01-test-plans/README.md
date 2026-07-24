# Test Plan

## Project Information

| Item | Details |
|------|---------|
| Project | OrangeHRM Demo |
| Testing Type | Manual Testing |
| Tester | Nurrohmi Zaki |
| Version | 2.0 |
| Status | In Progress |

---

# Version History

| Version | Description |
|----------|-------------|
| 1.0 | Initial Test Plan |
| 2.0 | Added Product Risk Analysis, Risk Mitigation Strategy, Test Prioritization, Deliverables, Assumptions, and Constraints |

---

# 1. Introduction

This document describes the overall testing strategy for the OrangeHRM Demo application.

The objective of this test plan is to define the testing scope, testing approach, priorities, schedule, and expected deliverables before the execution phase begins.

---

# 2. Objectives

The objectives of this testing are:

- Verify that core business features work correctly.
- Detect functional defects before release.
- Validate the application against expected business requirements.
- Reduce product risks through structured manual testing.

---

# 3. Scope

## In Scope

The following modules will be covered:

- Login
- Forgot Password
- Dashboard
- Admin
- PIM
- Leave
- Time
- Recruitment
- My Info
- Performance
- Directory
- Maintenance
- Claim
- Buzz
- Profile

## Out of Scope

The following testing activities are excluded:

- Performance Testing
- Security Testing
- Mobile Testing
- API Testing
- Automation Testing
- Source Code Review

---

# 4. Test Environment

| Item | Details |
|------|---------|
| Application | OrangeHRM Demo |
| Browser | Google Chrome (Latest Version) |
| Internet | Stable Internet Connection |
| Operating System | Windows 11 |
| Tester | Nurrohmi Zaki |

---

# 5. Test Strategy

Testing will be performed manually using a risk-based testing approach.

Activities include:

- Exploratory Testing
- Functional Testing
- Positive Testing
- Negative Testing
- Regression Testing (if required)

Priority will be given to business-critical features.

---

# 6. Entry Criteria

Testing can begin when:

- The application is accessible.
- Test environment is ready.
- Administrator account is available.
- Testing scope has been defined.
- Test Plan has been approved.

---

# 7. Exit Criteria

Testing will be completed when:

- All planned test cases have been executed.
- Critical defects have been reported.
- Testing objectives have been achieved.
- Test Summary Report has been completed.

---

# 8. Product Risk Analysis

The following risks were identified during the exploration phase.

| Feature | Potential Risk | Impact | Priority |
|----------|----------------|--------|----------|
| Login | User cannot access the system | High | High |
| User Management | User creation or deletion fails | High | High |
| PIM | Employee information is stored incorrectly | High | High |
| Leave | Incorrect leave calculation | High | High |
| Time | Attendance records are inaccurate | Medium | Medium |
| Recruitment | Candidate information is lost | Medium | Medium |
| Performance | KPI or review data is incorrect | Medium | Medium |
| Buzz | Social feed cannot create posts | Low | Low |

---

# 9. Risk Mitigation Strategy

| Risk | Mitigation |
|------|------------|
| Authentication failure | Perform smoke testing before execution |
| Employee data corruption | Prioritize CRUD and regression testing |
| Leave calculation errors | Create positive and negative test cases |
| Search functionality issues | Test multiple keyword combinations |
| Configuration changes | Execute regression testing after configuration updates |

---

# 10. Test Prioritization

Testing follows a risk-based approach.

## High Priority

- Login
- User Management
- PIM
- Leave

## Medium Priority

- Time
- Recruitment
- Performance
- Directory
- Maintenance
- Claim

## Low Priority

- Buzz
- Corporate Branding
- About
- Support

---

# 11. Test Deliverables

The following artifacts will be produced during this project.

- Test Plan
- Application Analysis
- Test Scenario
- Test Cases
- Test Data
- Bug Reports
- Test Execution Report
- Test Summary Report

---

# 12. Assumptions

The following assumptions apply during testing.

- OrangeHRM Demo remains available.
- Administrator account is accessible.
- Stable internet connection.
- No major system changes during testing.
- Testing is performed using a desktop browser.

---

# 13. Constraints

The following limitations apply.

- Source code is unavailable.
- Database access is unavailable.
- Only publicly available demo features are tested.
- Performance and security testing are excluded.

---

# 14. Test Schedule

| Phase | Status |
|--------|--------|
| Application Analysis | Completed |
| Test Planning | In Progress |
| Test Scenario | Planned |
| Test Case Design | Planned |
| Test Execution | Planned |
| Bug Reporting | Planned |
| Test Summary | Planned |

---

# Conclusion

This Test Plan provides the overall strategy for manually testing the OrangeHRM Demo application.

The testing process will continue by creating detailed Test Scenarios, Test Cases, executing manual testing, documenting defects, and producing the final Test Summary Report.
