# OrangeHRM Manual Testing Test Plan

## Project Information

| Item | Details |
|------|---------|
| Project | OrangeHRM Demo |
| Testing Type | Manual Functional Testing |
| Tester | Nurrohmi Zaki |
| Version | 3.0 |
| Status | Completed |

---

# Version History

| Version | Description |
|----------|-------------|
| 1.0 | Initial Test Plan |
| 2.0 | Added Product Risk Analysis, Risk Mitigation Strategy, Test Prioritization, Deliverables, Assumptions, and Constraints |
| 3.0 | Finalized project scope and updated documentation after project completion |

---

# 1. Introduction

This document defines the testing strategy used throughout the OrangeHRM Manual Testing project.

The purpose of this Test Plan is to document the project scope, testing approach, priorities, environment, deliverables, and execution strategy before manual testing activities were performed.

This document also serves as a reference for the completed Software Testing Life Cycle (STLC) implemented throughout this project.

---

# 2. Objectives

The objectives of this project are to:

- Verify that selected business-critical features function correctly.
- Detect functional defects through structured manual testing.
- Validate application behavior against expected business requirements.
- Demonstrate a professional manual testing workflow.
- Produce complete QA documentation following industry-standard STLC practices.

---

# 3. Scope

## In Scope

The following modules are included in this completed manual testing project:

- Authentication - Login
- Admin - User Management
- Admin - Job Titles
- Admin - Organization Locations

These modules provide representative coverage of common administrative workflows including authentication, CRUD operations, validation, search functionality, configuration management, and administrative data maintenance.

---

## Out of Scope

The following testing activities are excluded from this project:

- Performance Testing
- Security Testing
- Mobile Testing
- API Testing
- Automation Testing
- Source Code Review
- Database Validation

---

# 4. Test Environment

| Item | Details |
|------|---------|
| Application | OrangeHRM Demo |
| Browser | Google Chrome (Latest Version) |
| Operating System | Windows 11 |
| Internet | Stable Internet Connection |
| Tester | Nurrohmi Zaki |

---

# 5. Test Strategy

Testing was performed manually using a **Risk-Based Testing** approach.

The testing activities included:

- Functional Testing
- Manual Testing
- Positive Testing
- Negative Testing
- Exploratory Testing
- Validation Testing
- Regression Testing (where applicable)

Business-critical features were prioritized throughout the execution phase.

---

# 6. Entry Criteria

Testing could begin when:

- Application was accessible.
- Test environment was prepared.
- Administrator account was available.
- Testing scope was approved.
- Test Plan was completed.

---

# 7. Exit Criteria

Testing was considered complete when:

- All planned test cases were executed.
- Critical defects were documented.
- Testing objectives were achieved.
- Test Summary Report was completed.
- Test execution results were documented in Qase.io.

---

# 8. Product Risk Analysis

The following product risks were identified during project planning.

| Feature | Potential Risk | Impact | Priority |
|----------|----------------|--------|----------|
| Login | Users cannot access the system | High | High |
| User Management | User creation or deletion fails | High | High |
| Job Titles | Incorrect job title configuration | Medium | Medium |
| Organization Locations | Organization data becomes inconsistent | Medium | Medium |

---

# 9. Risk Mitigation Strategy

| Risk | Mitigation |
|------|------------|
| Authentication failure | Execute smoke testing before detailed testing |
| User management issues | Prioritize CRUD validation |
| Invalid configuration | Perform positive and negative testing |
| Search functionality defects | Test multiple search conditions |
| Configuration updates | Execute regression testing after changes |

---

# 10. Test Prioritization

Testing followed a Risk-Based Testing approach.

## High Priority

- Login
- User Management

## Medium Priority

- Job Titles
- Organization Locations

## Low Priority

No low-priority modules were included in the project scope.

---

# 11. Test Deliverables

The following QA artifacts were produced during this project.

- Project Overview
- Application Analysis
- Test Plan
- Test Scenarios
- Test Cases
- Test Execution Reports
- Test Summary Report
- Bug Reports
- Testing Evidence
- Qase.io Test Management Documentation

---

# 12. Assumptions

The following assumptions applied during testing.

- OrangeHRM Demo remained accessible.
- Administrator account remained available.
- Stable internet connection was maintained.
- No major application updates occurred during testing.
- Testing was performed using a desktop browser.

---

# 13. Constraints

The following project limitations applied.

- Source code was unavailable.
- Database access was unavailable.
- Only publicly available demo features were tested.
- Performance testing was excluded.
- Security testing was excluded.

---

# 14. Test Schedule

| Phase | Status |
|--------|--------|
| Application Analysis | Completed |
| Test Planning | Completed |
| Test Scenario Design | Completed |
| Test Case Design | Completed |
| Manual Test Execution | Completed |
| Evidence Collection | Completed |
| Bug Reporting | Completed |
| Test Summary Report | Completed |
| Qase Test Management | Completed |

---

# 15. Testing Outcome

The completed project achieved the following outcomes:

| Metric | Result |
|---------|--------:|
| Modules Tested | 4 |
| Test Cases | 124 |
| Test Executions | 124 |
| Passed | 123 |
| Failed | 1 |
| Pass Rate | 99.19% |
| Bug Reports | 1 |

---

# Conclusion

This Test Plan documents the overall testing strategy implemented throughout the completed OrangeHRM Manual Testing project.

All planned testing activities were successfully completed, including planning, test design, execution, evidence collection, defect reporting, and test management using Qase.io.

This repository serves as a completed Manual Testing portfolio demonstrating a structured Quality Assurance workflow following industry-standard Software Testing Life Cycle (STLC) practices.
