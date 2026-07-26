# Admin - User Management Test Scenarios

## Overview

This document defines the high-level test scenarios for the **User Management** module in the OrangeHRM Demo application.

The objective is to ensure that administrators can search, create, update, and delete user accounts while maintaining data integrity and proper validation.

---

## Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | User Management |
| Test Type | Manual Functional Testing |
| Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

# Test Scenarios

| Scenario ID | Feature | Test Scenario | Priority |
|--------------|---------|---------------|----------|
| TS_ADMIN_USER_001 | User List | Verify User Management page is displayed successfully | High |
| TS_ADMIN_USER_002 | User List | Verify all required table columns are displayed | High |
| TS_ADMIN_USER_003 | User List | Verify Edit action is available for each user | Medium |
| TS_ADMIN_USER_004 | User List | Verify Delete action is available for each user | Medium |
| TS_ADMIN_USER_005 | Search | Verify search by Username | High |
| TS_ADMIN_USER_006 | Search | Verify search by User Role | High |
| TS_ADMIN_USER_007 | Search | Verify search by Employee Name | High |
| TS_ADMIN_USER_008 | Search | Verify search by Status | High |
| TS_ADMIN_USER_009 | Search | Verify search using multiple filters | High |
| TS_ADMIN_USER_010 | Search | Verify search with non-existing data | Medium |
| TS_ADMIN_USER_011 | Search | Verify Reset button clears all search filters | Medium |
| TS_ADMIN_USER_012 | Add User | Verify administrator can add a new user with valid data | High |
| TS_ADMIN_USER_013 | Add User | Verify required field validation when mandatory fields are empty | High |
| TS_ADMIN_USER_014 | Add User | Verify Employee Name only accepts existing employees | High |
| TS_ADMIN_USER_015 | Add User | Verify Username minimum length validation | High |
| TS_ADMIN_USER_016 | Add User | Verify Password and Confirm Password must match | High |
| TS_ADMIN_USER_017 | Add User | Verify Cancel button returns to User Management page | Medium |
| TS_ADMIN_USER_018 | Add User | Verify success notification after adding a user | Medium |
| TS_ADMIN_USER_019 | Edit User | Verify administrator can edit user information | High |
| TS_ADMIN_USER_020 | Edit User | Verify Username can be updated | Medium |
| TS_ADMIN_USER_021 | Edit User | Verify User Role can be updated | Medium |
| TS_ADMIN_USER_022 | Edit User | Verify Employee Name can be updated | Medium |
| TS_ADMIN_USER_023 | Edit User | Verify Status can be updated | Medium |
| TS_ADMIN_USER_024 | Edit User | Verify Change Password option displays Password fields | High |
| TS_ADMIN_USER_025 | Edit User | Verify password update with valid values | High |
| TS_ADMIN_USER_026 | Edit User | Verify password confirmation validation | High |
| TS_ADMIN_USER_027 | Edit User | Verify Cancel button discards changes | Medium |
| TS_ADMIN_USER_028 | Edit User | Verify success notification after updating a user | Medium |
| TS_ADMIN_USER_029 | Delete User | Verify delete confirmation dialog appears | High |
| TS_ADMIN_USER_030 | Delete User | Verify user can be deleted successfully | High |
| TS_ADMIN_USER_031 | Delete User | Verify Cancel button closes confirmation dialog | Medium |
| TS_ADMIN_USER_032 | Delete User | Verify success notification after deleting a user | Medium |
| TS_ADMIN_USER_033 | Sorting | Verify Username column sorting (Ascending) | Medium |
| TS_ADMIN_USER_034 | Sorting | Verify Username column sorting (Descending) | Medium |
| TS_ADMIN_USER_035 | Sorting | Verify User Role column sorting | Medium |
| TS_ADMIN_USER_036 | Sorting | Verify Employee Name column sorting | Medium |
| TS_ADMIN_USER_037 | Sorting | Verify Status column sorting | Medium |
| TS_ADMIN_USER_038 | Validation | Verify Username accepts minimum 5 characters | High |
| TS_ADMIN_USER_039 | Validation | Verify leading and trailing spaces handling | Medium |
| TS_ADMIN_USER_040 | Validation | Verify invalid Employee Name cannot be submitted | High |

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| User List | ✅ |
| Search | ✅ |
| Add User | ✅ |
| Edit User | ✅ |
| Change Password | ✅ |
| Delete User | ✅ |
| Sorting | ✅ |
| Validation | ✅ |

---

# Notes

- These scenarios describe high-level business flows only.
- Detailed execution steps will be documented in the Test Cases document.
- Actual execution results will be documented in the Test Execution document.
- Any defects identified during execution will be recorded in the Bug Report document.
