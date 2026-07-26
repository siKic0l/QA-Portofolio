# Admin User Management Test Execution

## Overview

This document records the execution results of all manual test cases for the **User Management** feature under the **Admin** module in the OrangeHRM Demo application.

The purpose of this document is to track execution progress, record actual testing results, provide supporting evidence, and document any defects identified during testing.

---

# Execution Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | User Management |
| Test Type | Manual Functional Testing |
| Tester | Nurrohmi Zaki |
| Environment | Windows 11 • Google Chrome (Latest) |
| Execution Date | *To be updated* |
| Execution Status | Not Started |

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_ADMIN_USER_001 | Verify User Management Page Loads Successfully | User Management page loads correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_002 | Verify User Table is Displayed Correctly | User table displays all required columns | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_003 | Verify Add Button is Displayed | Add User page is opened successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_004 | Verify Edit Button is Available | Edit button is available for every user | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_005 | Verify Delete Button is Available | Delete button is available for every user | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_006 | Search User by Valid Username | Matching user is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_007 | Search User by Invalid Username | No matching records are found | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_008 | Search User by User Role | Users are filtered correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_009 | Search User by Employee Name | Matching employee is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_010 | Search User by Status | Users are filtered by selected status | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_011 | Search User Using Multiple Filters | Search results satisfy all selected filter criteria | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_012 | Verify Reset Button Clears Search Filters | All search fields are cleared and default values are restored | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_013 | Search with Empty Filters | All user records are displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_014 | Add User with Valid Information | User is created successfully and appears in the User List | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_015 | Add User with Empty Required Fields | Required validation messages are displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_016 | Verify Employee Name Autocomplete | Matching employee suggestions are displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_017 | Verify Invalid Employee Name Cannot Be Selected | Validation message is displayed and user is not created | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_018 | Verify Username Minimum Length Validation | Username validation message is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_019 | Verify Password and Confirm Password Validation | Password mismatch validation is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_020 | Cancel User Creation | User creation is cancelled and no new user is added | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_021 | Edit Username Successfully | Username is updated successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_022 | Edit User Role Successfully | User Role is updated successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_023 | Edit Employee Name Successfully | Employee Name is updated successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_024 | Edit Status Successfully | Status is updated successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_025 | Verify Change Password Checkbox | Password and Confirm Password fields are displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_026 | Change Password Successfully | Password is updated successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_027 | Verify Password Confirmation Validation During Edit | Password mismatch validation is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_028 | Verify Required Password Fields After Enabling Change Password | Required validation messages are displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_029 | Cancel User Update | Changes are discarded | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_030 | Verify Success Toast After Updating User | Success toast notification is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_031 | Delete User Successfully | User is deleted successfully | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_032 | Cancel User Deletion | User remains in the User List | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_033 | Verify Delete Confirmation Dialog | Confirmation dialog is displayed | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_034 | Verify Username Column Sorting | Username column is sorted correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_035 | Verify User Role Column Sorting | User Role column is sorted correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_036 | Verify Employee Name Column Sorting | Employee Name column is sorted correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_037 | Verify Status Column Sorting | Status column is sorted correctly | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_038 | Verify Username with Minimum Allowed Length | Username containing exactly five characters is accepted | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_039 | Verify Leading and Trailing Spaces in Username | Username is processed according to validation rules | - | ⏳ Not Executed | - | - |
| TC_ADMIN_USER_040 | Verify Employee Name Only Accepts Existing Employees | Only existing employees can be selected | - | ⏳ Not Executed | - | - |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 40 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 40 |
| Pass Rate | 0% |

---

# Notes

- Test execution has **not** been performed yet.
- Actual Result, Status, Evidence, and Bug ID will be updated after each test case is executed.
- Failed test cases will be linked to the corresponding Bug Report.
- Screenshots and supporting evidence will be stored in the **evidence/admin-user-management/** directory.
