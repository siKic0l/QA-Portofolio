# Login Test Cases

## Overview

This document contains the manual test cases for the **Login** feature of the OrangeHRM Demo application.

The objective is to verify that the authentication process behaves correctly under normal, invalid, boundary, and validation state conditions.

---

# Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Authentication |
| Feature | Login |
| Test Type | Functional Testing |
| Test Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

# Preconditions

Before executing the test cases, ensure that:

- OrangeHRM Demo website is accessible.
- User is on the Login page.
- Test account is available.
- Internet connection is stable.

---

# Test Data

| Username | Password | Description |
|----------|----------|-------------|
| Admin | admin123 | Valid credentials |
| Admin | wrongpassword | Invalid password |
| wronguser | admin123 | Invalid username |
| *(empty)* | admin123 | Empty username |
| Admin | *(empty)* | Empty password |
| *(empty)* | *(empty)* | Empty username and password |

---

# Test Cases

---

## TC_LOGIN_001 - Login with Valid Credentials

**Priority**

High

**Objective**

Verify that users can successfully log in using valid credentials.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the OrangeHRM Login page. |
| 2 | Enter a valid username. |
| 3 | Enter a valid password. |
| 4 | Click **Login**. |

### Expected Result

- User is successfully authenticated.
- Dashboard page is displayed.
- User session is created.

---

## TC_LOGIN_002 - Login with Invalid Password

**Priority**

High

**Objective**

Verify that login is rejected when the password is incorrect.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Enter a valid username. |
| 3 | Enter an invalid password. |
| 4 | Click **Login**. |

### Expected Result

- Login fails.
- **"Invalid credentials"** message is displayed.
- User remains on the Login page.
- User is not authenticated.

---

## TC_LOGIN_003 - Login with Invalid Username

**Priority**

High

**Objective**

Verify that login is rejected when the username does not exist.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Enter an invalid username. |
| 3 | Enter a valid password. |
| 4 | Click **Login**. |

### Expected Result

- Login fails.
- **"Invalid credentials"** message is displayed.
- User remains on the Login page.
- User is not authenticated.

---

## TC_LOGIN_004 - Login with Empty Username

**Priority**

High

**Objective**

Verify validation when the Username field is empty.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Leave the Username field empty. |
| 3 | Enter a valid password. |
| 4 | Click **Login**. |

### Expected Result

- **"Required"** validation message is displayed below the Username field.
- Login request is not submitted.

---

## TC_LOGIN_005 - Login with Empty Password

**Priority**

High

**Objective**

Verify validation when the Password field is empty.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Enter a valid username. |
| 3 | Leave the Password field empty. |
| 4 | Click **Login**. |

### Expected Result

- **"Required"** validation message is displayed below the Password field.
- Login request is not submitted.

---

## TC_LOGIN_006 - Login with Empty Username and Password

**Priority**

High

**Objective**

Verify validation when both Username and Password fields are empty.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Leave the Username field empty. |
| 3 | Leave the Password field empty. |
| 4 | Click **Login**. |

### Expected Result

- **"Required"** validation message is displayed for both Username and Password fields.
- Login request is not submitted.

---

## TC_LOGIN_007 - Verify Password Masking

**Priority**

Medium

**Objective**

Verify that password characters are hidden while typing.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Enter any password. |

### Expected Result

- Password characters are masked.
- The entered password is not visible.

---

## TC_LOGIN_008 - Forgot Password Navigation

**Priority**

Medium

**Objective**

Verify that the **Forgot your password?** link redirects users correctly.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Click **Forgot your password?**. |

### Expected Result

- User is redirected to the Reset Password page.

---

## TC_LOGIN_009 - Login Using Enter Key

**Priority**

Medium

**Objective**

Verify that pressing the **Enter** key submits the login form.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Enter a valid username. |
| 2 | Enter a valid password. |
| 3 | Press the **Enter** key. |

### Expected Result

- Login request is submitted.
- User is successfully logged in.
- Dashboard page is displayed.

---

## TC_LOGIN_010 - Username with Leading and Trailing Spaces

**Priority**

Low

**Objective**

Verify how the application handles leading and trailing whitespace in the Username field.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Enter a valid username with leading and trailing spaces. |
| 2 | Enter a valid password. |
| 3 | Click **Login**. |

### Expected Result

- Leading and trailing whitespace is automatically trimmed.
- User is successfully authenticated.
- Dashboard page is displayed.

---

## TC_LOGIN_011 - Verify Validation Message State After Previous Failed Authentication

**Priority**

Medium

**Objective**

Verify that the previous authentication error message is cleared when required field validation is triggered after a failed login attempt.

### Test Steps

| Step | Action |
|------|--------|
| 1 | Open the Login page. |
| 2 | Enter a valid username (**Admin**). |
| 3 | Enter an invalid password (**wrongpassword**). |
| 4 | Click **Login**. |
| 5 | Verify that the **"Invalid credentials"** message is displayed. |
| 6 | Clear the Password field, leaving it empty. |
| 7 | Click **Login** again. |

### Expected Result

- Only the **"Required"** validation message is displayed.
- The previous **"Invalid credentials"** message is cleared.
- Login request is not submitted because required field validation is triggered.

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| Valid Login | ✅ |
| Invalid Username | ✅ |
| Invalid Password | ✅ |
| Empty Field Validation | ✅ |
| Password Masking | ✅ |
| Forgot Password | ✅ |
| Keyboard Interaction | ✅ |
| Username Whitespace Handling | ✅ |
| Validation State Management | ✅ |

---

# Notes

- Test cases define the expected behavior of the Login feature.
- Test execution results, evidence, and bug reports are documented separately in the **Test Execution** and **Bug Reports** folders.
- TC_LOGIN_011 was added during exploratory testing after identifying an unexpected validation state behavior.
