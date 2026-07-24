# Login Test Execution

## Overview

This document records the execution results of all manual test cases for the **Login** module of the OrangeHRM Demo application.

The purpose of this document is to verify that the Login functionality behaves as expected, document the execution results, and provide traceability between test cases, evidence, and reported defects.

---

# Execution Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Authentication - Login |
| Test Type | Manual Functional Testing |
| Tester | Nurrohmi Zaki |
| Environment | Windows 11 • Google Chrome (Latest) |
| Browser | Google Chrome (Latest) |
| Execution Date | 24 July 2026 |
| Execution Status | ✅ Completed |

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_LOGIN_001 | Login with valid credentials | User successfully logs in and is redirected to Dashboard. | User successfully logged in and was redirected to Dashboard. | ✅ PASS | ..evidence/Login/TC_LOGIN_001_PASS.png | - |
| TC_LOGIN_002 | Login with invalid password | Error message is displayed. | "Invalid credentials" message displayed correctly. | ✅ PASS | evidence/Login/TC_LOGIN_002_PASS.png | - |
| TC_LOGIN_003 | Login with invalid username | Error message is displayed. | "Invalid credentials" message displayed correctly. | ✅ PASS | evidence/Login/TC_LOGIN_003_PASS.png | - |
| TC_LOGIN_004 | Login with empty username | "Required" validation message is displayed. | "Required" validation message displayed correctly. | ✅ PASS | evidence/Login/TC_LOGIN_004_PASS.png | - |
| TC_LOGIN_005 | Login with empty password | "Required" validation message is displayed. | "Required" validation message displayed correctly. | ✅ PASS | evidence/Login/TC_LOGIN_005_PASS.png | - |
| TC_LOGIN_006 | Login with empty username and password | "Required" validation messages are displayed. | "Required" validation messages displayed correctly. | ✅ PASS | evidence/Login/TC_LOGIN_006_PASS.png | - |
| TC_LOGIN_007 | Verify password masking | Password characters are masked while typing. | Password input was masked correctly. | ✅ PASS | evidence/Login/TC_LOGIN_007_PASS.png | - |
| TC_LOGIN_008 | Forgot Password navigation | User is redirected to Reset Password page. | Successfully redirected to Reset Password page. | ✅ PASS | evidence/Login/TC_LOGIN_008_PASS.png | - |
| TC_LOGIN_009 | Login using Enter key | Login request is submitted successfully. | Login was successfully submitted using the Enter key. | ✅ PASS | evidence/Login/TC_LOGIN_009_PASS.png | - |
| TC_LOGIN_010 | Username with leading/trailing spaces | Username is processed correctly. | Leading and trailing whitespace was automatically trimmed and login succeeded. | ✅ PASS | evidence/Login/TC_LOGIN_010_PASS.png | - |
| TC_LOGIN_011 | Verify validation message state after previous failed authentication | Previous "Invalid credentials" message should be cleared, and only "Required" validation should be displayed. | Previous "Invalid credentials" message remained visible together with the "Required" validation message. | ❌ FAIL | evidence/Login/TC_LOGIN_011_FAIL.png | BUG_LOGIN_001 |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 11 |
| Passed | 10 |
| Failed | 1 |
| Blocked | 0 |
| Not Executed | 0 |
| Pass Rate | 90.91% |
| Bugs Found | 1 |

---

# Defects Found

| Bug ID | Title | Severity | Priority | Status |
|--------|-------|----------|----------|--------|
| BUG_LOGIN_001 | Previous authentication error message remains visible after Required field validation is triggered | Low | Medium | Open |

---

# Execution Notes

- All planned login test cases (TC_LOGIN_001 – TC_LOGIN_010) passed successfully.
- During additional validation state testing, one UI validation issue was identified.
- The issue occurs when a failed login attempt is followed by submitting the form with one or more required fields left empty.
- The defect has been documented as **05-bug-reports/Login/BUG_LOGIN_001**.

---

# Conclusion

The Login functionality of the OrangeHRM Demo application generally works as expected. All planned functional test cases passed successfully. One minor UI validation issue related to validation message persistence was identified during additional exploratory testing. The issue does not prevent users from logging in but may cause confusion due to multiple validation messages being displayed simultaneously.
