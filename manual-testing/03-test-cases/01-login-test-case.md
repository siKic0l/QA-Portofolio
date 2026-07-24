# Login Test Cases

## Overview

This document contains the manual test cases for the **Login** feature of the OrangeHRM Demo application.

The objective is to verify that the authentication process behaves correctly under normal, invalid, and boundary conditions.

---

## Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Authentication |
| Feature | Login |
| Test Type | Functional Testing |
| Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

## Preconditions

Before executing the test cases, ensure that:

- OrangeHRM Demo website is accessible.
- User is on the Login page.
- Test account is available.
- Internet connection is stable.

---

## Test Data

| Username | Password | Description |
|----------|----------|-------------|
| Admin | admin123 | Valid credential |
| Admin | wrongpassword | Invalid password |
| wronguser | admin123 | Invalid username |
| *(empty)* | admin123 | Empty username |
| Admin | *(empty)* | Empty password |
| *(empty)* | *(empty)* | Empty credentials |

---

# Test Cases

---

## TC_LOGIN_001 - Login with Valid Credentials

**Priority**

High

**Objective**

Verify that users can log in using valid credentials.

### Test Steps

| Step | Action |
|------|--------|
|1|Open OrangeHRM Login page|
|2|Enter valid username|
|3|Enter valid password|
|4|Click **Login**|

### Expected Result

- User successfully logs in.
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
|1|Open Login page|
|2|Enter valid username|
|3|Enter invalid password|
|4|Click Login|

### Expected Result

- Login fails.
- Error message is displayed.
- User remains on Login page.

---

## TC_LOGIN_003 - Login with Invalid Username

**Priority**

High

**Objective**

Verify that login fails when the username does not exist.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Enter invalid username|
|3|Enter valid password|
|4|Click Login|

### Expected Result

- Login fails.
- Error message is displayed.
- User remains on Login page.

---

## TC_LOGIN_004 - Login with Empty Username

**Priority**

High

**Objective**

Verify validation when username is empty.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Leave Username empty|
|3|Enter password|
|4|Click Login|

### Expected Result

- Validation message appears.
- Login is not processed.

---

## TC_LOGIN_005 - Login with Empty Password

**Priority**

High

**Objective**

Verify validation when password is empty.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Enter username|
|3|Leave Password empty|
|4|Click Login|

### Expected Result

- Validation message appears.
- Login is not processed.

---

## TC_LOGIN_006 - Login with Empty Username and Password

**Priority**

High

**Objective**

Verify validation when both fields are empty.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Leave Username empty|
|3|Leave Password empty|
|4|Click Login|

### Expected Result

- Required field validation appears.
- Login is not processed.

---

## TC_LOGIN_007 - Verify Password Masking

**Priority**

Medium

**Objective**

Verify that password characters are hidden while typing.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Enter password|

### Expected Result

- Password characters are masked.
- Actual password is not visible.

---

## TC_LOGIN_008 - Forgot Password Navigation

**Priority**

Medium

**Objective**

Verify that the Forgot Password link redirects users correctly.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Login page|
|2|Click **Forgot your password?**|

### Expected Result

- Reset Password page is displayed.

---

## TC_LOGIN_009 - Login Using Enter Key

**Priority**

Medium

**Objective**

Verify that pressing Enter submits the login form.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter valid username|
|2|Enter valid password|
|3|Press Enter|

### Expected Result

- Login is successful.
- Dashboard page is displayed.

---

## TC_LOGIN_010 - Username with Leading or Trailing Spaces

**Priority**

Low

**Objective**

Verify how the application handles whitespace in username input.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter username with leading/trailing spaces|
|2|Enter valid password|
|3|Click Login|

### Expected Result

- System trims unnecessary spaces **or**
- Displays appropriate validation message.

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| Valid Login | ✅ |
| Invalid Username | ✅ |
| Invalid Password | ✅ |
| Empty Validation | ✅ |
| Password Masking | ✅ |
| Forgot Password | ✅ |
| Keyboard Interaction | ✅ |
| Input Validation | ✅ |

---

# Notes

- Test execution has **not** been performed yet.
- Actual Result, Status, Evidence, and Bug Reports will be documented during the Test Execution phase.
