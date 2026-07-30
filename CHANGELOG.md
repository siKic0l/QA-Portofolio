# Changelog

All notable changes to this QA Portfolio are documented in this file.

This project follows **Semantic Versioning (SemVer)** to record significant updates to testing artifacts, documentation, repository structure, and QA workflow.

---

# v1.2.0 - Qase Integration & Repository Enhancement

**Release Date:** July 30, 2026

## Added

### Test Management

- Integrated **Qase.io** as the Test Management System
- Created Test Suites for all completed OrangeHRM modules
- Imported all manual test cases into Qase
- Executed manual test runs in Qase
- Published Qase Public Test Report

### Documentation

- Added Qase documentation
- Added Test Suites documentation
- Added Test Runs documentation
- Added Test Metrics documentation

### Repository Improvements

- Redesigned main README
- Updated Project Overview
- Added repository statistics
- Added portfolio highlights
- Added QA workflow documentation
- Improved repository structure
- Added Qase screenshots

---

## Repository Metrics

| Item | Total |
|------|------:|
| Applications | 1 |
| Modules Completed | 4 |
| Test Suites | 4 |
| Test Cases | 124 |
| Test Executions | 124 |
| Passed | 123 |
| Failed | 1 |
| Bug Reports | 1 |
| Evidence Collected | 124+ Screenshots |

---

# v1.1.0 - OrangeHRM Admin Modules Completed

**Release Date:** July 27, 2026

## Added

### Documentation

#### Admin - User Management

- Test Scenarios
- Test Cases
- Test Execution Report

#### Admin - Job Titles

- Test Scenarios
- Test Cases
- Test Execution Report

#### Admin - Organization - Locations

- Test Scenarios
- Test Cases
- Test Execution Report

### Reports

- OrangeHRM Test Summary Report

### Evidence

- User Management execution evidence
- Job Titles execution evidence
- Organization Locations execution evidence

### Repository Improvements

- Updated README
- Updated Project Overview
- Improved documentation consistency

---

## Testing Summary

| Module | Status |
|---------|--------|
| Authentication - Login | Completed |
| Admin - User Management | Completed |
| Admin - Job Titles | Completed |
| Admin - Organization - Locations | Completed |

---

## Repository Metrics

| Item | Total |
|------|------:|
| Modules Completed | 4 |
| Test Scenario Documents | 4 |
| Test Case Documents | 4 |
| Test Execution Reports | 4 |
| Bug Reports | 1 |
| Evidence Collected | 124+ Screenshots |

---

# v1.0.0 - Authentication (Login) Module Completed

**Release Date:** July 20, 2026

## Added

### Documentation

- Project Overview
- Application Analysis
- Login Test Plan
- Login Test Scenarios
- Login Test Cases
- Login Test Execution Report

### Reports

- Login Bug Report

### Evidence

- Login execution evidence

---

## Testing Summary

| Metric | Result |
|--------|--------:|
| Test Cases | 11 |
| Passed | 10 |
| Failed | 1 |
| Bug Reports | 1 |

---

## Defects

### BUG_LOGIN_001

**Title**

Validation state inconsistency after failed authentication.

**Description**

After a failed login attempt displaying the **"Invalid credentials"** message, submitting the form again with an empty Password field displays both the previous authentication error and the **"Required"** validation message simultaneously.

**Expected Behavior**

The previous authentication error should be cleared when client-side required field validation is triggered.

**Status**

Open

---

# Upcoming

## Manual Testing

- Complete remaining OrangeHRM Admin features
- PIM Module
- Leave Module
- Time Module
- Recruitment Module
- Performance Module

---

## Quality Assurance

- API Testing with Postman
- SQL Database Validation
- Advanced Qase Test Management
- Cross-browser Testing

---

## Automation Testing

- Playwright
- Selenium
- API Test Automation
- GitHub Actions CI Integration

---

## Long-term Goal

Expand this portfolio by testing multiple real-world applications using:

- Manual Testing
- API Testing
- Database Testing
- Automation Testing
- Performance Testing

to demonstrate end-to-end Software Quality Assurance skills aligned with industry practices.
