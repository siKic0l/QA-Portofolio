# Login Test Scenarios

## Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Login |
| Prepared By | Nurrohmi Zaki |
| Test Type | Manual Testing |
| Version | 1.0 |

---

# Objective

The purpose of this document is to define high-level test scenarios for the Login module of OrangeHRM Demo. These scenarios serve as the foundation for creating detailed test cases during the test design phase.

---

# Assumptions

- User is on the OrangeHRM Login page.
- Application is accessible.
- Valid user credentials are available.
- Internet connection is stable.

---

# Test Scenarios

| Scenario ID | Scenario | Priority | Type |
|-------------|----------|----------|------|
| TS-LOGIN-001 | Verify user can login with valid username and valid password | High | Positive |
| TS-LOGIN-002 | Verify login fails when username is invalid | High | Negative |
| TS-LOGIN-003 | Verify login fails when password is invalid | High | Negative |
| TS-LOGIN-004 | Verify login fails when both username and password are invalid | High | Negative |
| TS-LOGIN-005 | Verify validation message when username is empty | High | Validation |
| TS-LOGIN-006 | Verify validation message when password is empty | High | Validation |
| TS-LOGIN-007 | Verify validation message when both fields are empty | High | Validation |
| TS-LOGIN-008 | Verify password field masks entered characters | Medium | UI / Security |
| TS-LOGIN-009 | Verify Forgot Password link redirects to Reset Password page | Medium | Navigation |
| TS-LOGIN-010 | Verify successful logout after login | High | Functional |
| TS-LOGIN-011 | Verify user cannot access Dashboard without authentication | High | Security |
| TS-LOGIN-012 | Verify login page is displayed after user logs out | Medium | Functional |
| TS-LOGIN-013 | Verify session is maintained after successful login | Medium | Session |
| TS-LOGIN-014 | Verify user is redirected to Dashboard after successful login | High | Functional |
| TS-LOGIN-015 | Verify appropriate error message is displayed after failed login | High | Error Handling |

---

# Scenario Coverage

| Category | Covered |
|----------|---------|
| Positive Testing | ✅ |
| Negative Testing | ✅ |
| Input Validation | ✅ |
| Navigation | ✅ |
| Session Management | ✅ |
| Authentication | ✅ |
| Basic Security | ✅ |
| UI Verification | ✅ |

---

# Notes

- These are high-level scenarios only.
- Detailed test steps, test data, expected results, and execution status will be documented in the Test Cases document.
