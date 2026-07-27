# OrangeHRM Manual Testing Summary Report

## Document Information

| Item | Value |
|------|-------|
| Project | OrangeHRM Demo |
| Application Type | Web-based Human Resource Management System (HRMS) |
| Test Type | Manual Functional Testing |
| Test Scope | Authentication & Admin Modules |
| Tester | Nurrohmi Zaki |
| Report Version | 1.0 |
| Report Date | July 27, 2026 |
| Status | Completed |

---

# Version History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | July 27, 2026 | Nurrohmi Zaki | Initial Test Summary Report |

---

# Overview

This report summarizes the manual testing activities performed on the OrangeHRM Demo application.

The testing process followed the Software Testing Life Cycle (STLC), including application analysis, test planning, test scenario design, test case design, execution, evidence collection, and defect reporting.

The objective of this report is to provide an overall assessment of the testing scope, execution results, coverage, and identified defects.

---

# Testing Scope

The following application modules were included in this testing cycle.

| Module | Feature | Status |
|---------|---------|--------|
| Authentication | Login | Completed |
| Admin | User Management | Completed |
| Admin | Job Titles | Completed |
| Admin | Organization - Locations | Completed |

---

# Test Artifacts

The following QA documentation was produced during this project.

- Project Overview
- Application Analysis
- Test Plan
- Test Scenarios
- Test Cases
- Test Execution Reports
- Bug Reports
- Testing Evidence

---

# Test Execution Summary

| Metric | Result |
|--------|--------:|
| Modules Tested | 4 |
| Test Scenarios | 100+ |
| Test Cases Executed | 120+ |
| Passed | 120+ |
| Failed | 1* |
| Blocked | 0 |
| Not Executed | 0 |
| Overall Pass Rate | >99% |

> *The single failed test case corresponds to a validation behavior observed during Login testing and was documented as a functional defect.*

---

# Bug Summary

| Bug ID | Module | Severity | Status |
|---------|--------|----------|--------|
| BUG_LOGIN_001 | Authentication - Login | Low | Open |

---

# Testing Coverage

The completed testing covered:

- Functional Testing
- User Interface Validation
- Form Validation
- CRUD Operations
- Search Functionality
- Sorting Functionality
- File Upload Validation
- Required Field Validation
- Duplicate Validation
- Business Rule Validation
- Exploratory Testing

---

# Testing Techniques Applied

The following software testing techniques were applied throughout the project:

- Black Box Testing
- Exploratory Testing
- Equivalence Partitioning
- Boundary Value Analysis (BVA)
- Error Guessing

---

# Test Environment

| Item | Value |
|------|-------|
| Operating System | Windows 11 |
| Browser | Google Chrome (Latest) |
| Application | OrangeHRM Demo |
| Testing Method | Manual Testing |

---

# Deliverables

The following deliverables are available within this repository.

| Deliverable | Status |
|-------------|--------|
| Project Overview | ✅ |
| Application Analysis | ✅ |
| Test Plan | ✅ |
| Test Scenarios | ✅ |
| Test Cases | ✅ |
| Test Execution Reports | ✅ |
| Testing Evidence | ✅ |
| Bug Reports | ✅ |

---

# Conclusion

The defined testing scope for the OrangeHRM Demo application has been completed successfully.

A total of four application features were tested using structured manual testing techniques following the Software Testing Life Cycle (STLC). Most functionalities behaved as expected and successfully passed the designed test cases.

One functional defect related to the Login validation state was identified during testing and documented in the Bug Report section. Apart from this issue, no critical defects were observed within the completed testing scope.

This repository demonstrates a complete manual testing workflow, including planning, documentation, execution, evidence collection, and defect reporting, and will continue to expand with additional application modules and testing methodologies.

---

# Future Improvements

The next phase of this portfolio will include:

- Additional OrangeHRM modules
- API Testing using Postman
- SQL Validation
- Test Management with Qase.io
- Automation Testing using Playwright
- CI/CD integration with GitHub Actions
