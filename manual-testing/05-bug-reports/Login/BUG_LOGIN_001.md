# BUG_LOGIN_001 - Previous Authentication Error Message Persists After Required Field Validation

## Bug Information

| Item | Value |
|------|-------|
| Bug ID | BUG_LOGIN_001 |
| Title | Previous authentication error message remains visible after required field validation is triggered |
| Module | Authentication - Login |
| Feature | Login Validation |
| Environment | OrangeHRM Demo |
| Browser | Google Chrome (Latest) |
| Operating System | Windows 11 |
| Severity | Low |
| Priority | Medium |
| Status | Open |
| Reported By | Nurrohmi Zaki |
| Report Date | 24 July 2026 |

---

# Description

After a failed login attempt, the application displays the **"Invalid credentials"** error message as expected.

However, when the user clears one or more required fields and submits the login form again, the previous **"Invalid credentials"** message remains visible together with the **"Required"** validation message.

Since the login request is not submitted when required field validation is triggered, the previous authentication error should be cleared before displaying the new validation message.

---

# Preconditions

- User is on the OrangeHRM Login page.
- A valid test account is available.

---

# Steps to Reproduce

1. Open the OrangeHRM Login page.
2. Enter a valid username (`Admin`).
3. Enter an invalid password.
4. Click **Login**.
5. Verify that the **"Invalid credentials"** message appears.
6. Clear the Password field.
7. Click **Login** again.

---

# Expected Result

- The previous **"Invalid credentials"** message is cleared.
- Only the **"Required"** validation message is displayed.
- The login request is not submitted.

---

# Actual Result

Both validation messages are displayed simultaneously:

- **Invalid credentials**
- **Required**

The previous authentication error message is not cleared even though the login request is blocked by client-side validation.

---

# Impact

Although this issue does not prevent users from logging in, it may confuse users because two different validation messages are displayed at the same time.

---

# Evidence

| File | Description |
|------|-------------|
| `TC_LOGIN_011_FAIL.png` | Screenshot showing both **"Invalid credentials"** and **"Required"** validation messages displayed simultaneously. |

---

# Root Cause Analysis (Assumption)

The authentication error state is not cleared before client-side required field validation is executed, causing the previous server-side validation message to persist.

> **Note:** This is an assumption based on observed application behavior. The actual root cause can only be confirmed by reviewing the application's source code.

---

# Recommendation

Clear any previous authentication error messages before performing client-side validation. When required field validation is triggered, only the corresponding validation message should be displayed.

---

# Related Test Case

| Test Case | Result |
|-----------|--------|
| TC_LOGIN_011 | ❌ FAIL |

---

# Attachments

- `../evidence/login/TC_LOGIN_011_FAIL.png`

## Severity Justification

The issue does not affect the core login functionality or data integrity. However, it creates an inconsistent user experience by displaying multiple validation messages simultaneously, which may confuse users.
