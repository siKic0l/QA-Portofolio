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
| Execution Date | July 27, 2026 |
| Execution Status | Completed |

---

# Execution Result

**40 / 40 Test Cases Passed**

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_ADMIN_USER_001 | Verify User Management Page Loads Successfully | User Management page loads correctly | User Management page loaded successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_001_PASS.png) | - |
| TC_ADMIN_USER_002 | Verify User Table is Displayed Correctly | User table displays all required columns | User table displayed all required columns correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_002_PASS.png) | - |
| TC_ADMIN_USER_003 | Verify Add Button is Displayed | Add User page is opened successfully | Add User page opened successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_003_PASS.png) | - |
| TC_ADMIN_USER_004 | Verify Edit Button is Available | Edit button is available for every user | Edit button was available for every user record. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_004_PASS.png) | - |
| TC_ADMIN_USER_005 | Verify Delete Button is Available | Delete button is available for every user | Delete button was available for every user record. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_005_PASS.png) | - |
| TC_ADMIN_USER_006 | Search User by Valid Username | Matching user is displayed | Matching user was displayed successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_006_PASS.png) | - |
| TC_ADMIN_USER_007 | Search User by Invalid Username | No matching records are found | No matching records were found. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_007_PASS.png) | - |
| TC_ADMIN_USER_008 | Search User by User Role | Users are filtered correctly | Users were filtered correctly by User Role. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_008_PASS.png) | - |
| TC_ADMIN_USER_009 | Search User by Employee Name | Matching employee is displayed | Matching employee was displayed successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_009_PASS.png) | - |
| TC_ADMIN_USER_010 | Search User by Status | Users are filtered by selected status | Users were filtered correctly by Status. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_010_PASS.png) | - |
| TC_ADMIN_USER_011 | Search User Using Multiple Filters | Search results satisfy all selected filter criteria | Search results matched all selected filter criteria. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_011_PASS.png) | - |
| TC_ADMIN_USER_012 | Verify Reset Button Clears Search Filters | All search fields are cleared and default values are restored | Reset button cleared all search filters successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_012_PASS.png) | - |
| TC_ADMIN_USER_013 | Search with Empty Filters | All user records are displayed | All user records were displayed successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_013_PASS.png) | - |
| TC_ADMIN_USER_014 | Add User with Valid Information | User is created successfully and appears in the User List | User was created successfully and appeared in the User List. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_014_PASS.png) | - |
| TC_ADMIN_USER_015 | Add User with Empty Required Fields | Required validation messages are displayed | Required validation messages were displayed correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_015_PASS.png) | - |
| TC_ADMIN_USER_016 | Verify Employee Name Autocomplete | Matching employee suggestions are displayed | Employee autocomplete suggestions worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_016_PASS.png) | - |
| TC_ADMIN_USER_017 | Verify Invalid Employee Name Cannot Be Selected | Validation message is displayed and user is not created | Invalid employee name could not be selected. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_017_PASS.png) | - |
| TC_ADMIN_USER_018 | Verify Username Minimum Length Validation | Username validation message is displayed | Username minimum length validation worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_018_PASS.png) | - |
| TC_ADMIN_USER_019 | Verify Password and Confirm Password Validation | Password mismatch validation is displayed | Password mismatch validation worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_019_PASS.png) | - |
| TC_ADMIN_USER_020 | Cancel User Creation | User creation is cancelled and no new user is added | User creation was cancelled successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_020_PASS.png) | - |
| TC_ADMIN_USER_021 | Edit Username Successfully | Username is updated successfully | Username was updated successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_021_PASS.png) | - |
| TC_ADMIN_USER_022 | Edit User Role Successfully | User Role is updated successfully | User Role was updated successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_022_PASS.png) | - |
| TC_ADMIN_USER_023 | Edit Employee Name Successfully | Employee Name is updated successfully | Employee Name was updated successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_023_PASS.png) | - |
| TC_ADMIN_USER_024 | Edit Status Successfully | Status is updated successfully | Status was updated successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_024_PASS.png) | - |
| TC_ADMIN_USER_025 | Verify Change Password Checkbox | Password and Confirm Password fields are displayed | Password fields were displayed successfully after enabling Change Password. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_025_PASS.png) | - |
| TC_ADMIN_USER_026 | Change Password Successfully | Password is updated successfully | Password was updated successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_026_PASS.png) | - |
| TC_ADMIN_USER_027 | Verify Password Confirmation Validation During Edit | Password mismatch validation is displayed | Password confirmation validation worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_027_PASS.png) | - |
| TC_ADMIN_USER_028 | Verify Required Password Fields After Enabling Change Password | Required validation messages are displayed | Required validation messages were displayed correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_028_PASS.png) | - |
| TC_ADMIN_USER_029 | Cancel User Update | Changes are discarded | User update was cancelled successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_029_PASS.png) | - |
| TC_ADMIN_USER_030 | Verify Success Toast After Updating User | Success toast notification is displayed | Success toast notification was displayed correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_030_PASS.png) | - |
| TC_ADMIN_USER_031 | Delete User Successfully | User is deleted successfully | User was deleted successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_031_PASS.png) | - |
| TC_ADMIN_USER_032 | Cancel User Deletion | User remains in the User List | User deletion was cancelled successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_032_PASS.png) | - |
| TC_ADMIN_USER_033 | Verify Delete Confirmation Dialog | Confirmation dialog is displayed | Delete confirmation dialog was displayed correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_033_PASS.png) | - |
| TC_ADMIN_USER_034 | Verify Username Column Sorting | Username column is sorted correctly | Username column sorting worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_034_PASS.png) | - |
| TC_ADMIN_USER_035 | Verify User Role Column Sorting | User Role column is sorted correctly | User Role column sorting worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_035_PASS.png) | - |
| TC_ADMIN_USER_036 | Verify Employee Name Column Sorting | Employee Name column is sorted correctly | Employee Name column sorting worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_036_PASS.png) | - |
| TC_ADMIN_USER_037 | Verify Status Column Sorting | Status column is sorted correctly | Status column sorting worked correctly. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_037_PASS.png) | - |
| TC_ADMIN_USER_038 | Verify Username with Minimum Allowed Length | Username containing exactly five characters is accepted | Username with minimum allowed length was accepted successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_038_PASS.png) | - |
| TC_ADMIN_USER_039 | Verify Leading and Trailing Spaces in Username | Username is processed according to validation rules | Username whitespace handling worked as expected. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_039_PASS.png) | - |
| TC_ADMIN_USER_040 | Verify Employee Name Only Accepts Existing Employees | Only existing employees can be selected | Only existing employees could be selected successfully. | PASS | [View Evidence](../evidence/Admin-User-Management/TC_ADMIN_USER_040_PASS.png) | - |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 0 |
| Pass Rate | **100%** |

---

# Notes

- All planned test cases were successfully executed.
- No functional defects were identified during the execution of the User Management module.
- All test cases passed successfully based on the expected application behavior.
- Supporting screenshots for each executed test case are available in the `evidence/Admin-User-Management/` directory.
