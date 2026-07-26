# Admin User Management Test Cases

## Overview

This document contains the manual test cases for the **User Management** feature under the **Admin** module of the OrangeHRM Demo application.

The objective is to verify that administrators can manage user accounts correctly, including viewing users, searching, sorting, creating, updating, and deleting user records while ensuring proper validation and system behavior.

---

# Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | User Management |
| Test Type | Functional Testing |
| Test Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

# Preconditions

Before executing the test cases, ensure that:

- OrangeHRM Demo website is accessible.
- User has successfully logged in as **Administrator**.
- User is on **Admin → User Management** page.
- Internet connection is stable.

---

# Test Data

| Field | Sample Value | Description |
|------|--------------|-------------|
| Username | Admin | Existing username |
| Username | InvalidUser | Non-existing username |
| User Role | Admin | Existing role |
| User Role | ESS | Existing role |
| Employee Name | Linda Anderson | Existing employee |
| Employee Name | Invalid Employee | Non-existing employee |
| Status | Enabled | Active account |
| Status | Disabled | Disabled account |
| Password | Admin123! | Valid password |
| Confirm Password | Admin123! | Matching password |

---

# Test Cases

---

## TC_ADMIN_USER_001 - Verify User Management Page Loads Successfully

**Priority**

High

**Objective**

Verify that the User Management page loads successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Navigate to **Admin → User Management**.|

### Expected Result

- User Management page is displayed successfully.
- Search section is visible.
- User table is displayed.
- Action buttons are available.

---

## TC_ADMIN_USER_002 - Verify User Table is Displayed Correctly

**Priority**

High

**Objective**

Verify that the user list displays all required columns.

### Test Steps

| Step | Action |
|------|--------|
|1|Open User Management page.|
|2|Observe the user table.|

### Expected Result

The table displays:

- Username
- User Role
- Employee Name
- Status
- Actions

---

## TC_ADMIN_USER_003 - Verify Add Button is Displayed

**Priority**

Medium

**Objective**

Verify that administrators can access the Add User page.

### Test Steps

| Step | Action |
|------|--------|
|1|Open User Management page.|
|2|Verify the **Add** button is displayed.|
|3|Click **Add**.|

### Expected Result

- Add User page is displayed.
- User creation form is available.

---

## TC_ADMIN_USER_004 - Verify Edit Button is Available

**Priority**

Medium

**Objective**

Verify that each user record provides an Edit action.

### Test Steps

| Step | Action |
|------|--------|
|1|Open User Management page.|
|2|Observe the Actions column.|

### Expected Result

- Every user row displays an Edit button.
- Edit button is clickable.

---

## TC_ADMIN_USER_005 - Verify Delete Button is Available

**Priority**

Medium

**Objective**

Verify that each user record provides a Delete action.

### Test Steps

| Step | Action |
|------|--------|
|1|Open User Management page.|
|2|Observe the Actions column.|

### Expected Result

- Every user row displays a Delete button.
- Delete button is clickable.

---

## TC_ADMIN_USER_006 - Search User by Valid Username

**Priority**

High

**Objective**

Verify that users can be searched using a valid username.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter an existing Username.|
|2|Click **Search**.|

### Expected Result

- Matching user is displayed.
- Search result matches the entered username.

---

## TC_ADMIN_USER_007 - Search User by Invalid Username

**Priority**

High

**Objective**

Verify system behavior when searching for a username that does not exist.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter a non-existing Username.|
|2|Click **Search**.|

### Expected Result

- No matching records are displayed.
- **No Records Found** message is shown.

---

## TC_ADMIN_USER_008 - Search User by User Role

**Priority**

High

**Objective**

Verify users can be filtered by User Role.

### Test Steps

| Step | Action |
|------|--------|
|1|Select a User Role from the dropdown.|
|2|Click **Search**.|

### Expected Result

- Only users with the selected role are displayed.

---

## TC_ADMIN_USER_009 - Search User by Employee Name

**Priority**

High

**Objective**

Verify users can be searched using Employee Name.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter an existing Employee Name.|
|2|Select the suggested employee from autocomplete.|
|3|Click **Search**.|

### Expected Result

- Matching employee account is displayed.
- Search result matches the selected employee.

---

## TC_ADMIN_USER_010 - Search User by Status

**Priority**

High

**Objective**

Verify users can be filtered by account status.

### Test Steps

| Step | Action |
|------|--------|
|1|Select **Enabled** or **Disabled** from Status dropdown.|
|2|Click **Search**.|

### Expected Result

- Only users with the selected status are displayed.

---

## TC_ADMIN_USER_011 - Search User Using Multiple Filters

**Priority**

High

**Objective**

Verify that the system returns users matching multiple search criteria simultaneously.

### Test Steps

| Step | Action |
|------|--------|
|1|Select a User Role.|
|2|Enter an existing Employee Name.|
|3|Select a Status.|
|4|Click **Search**.|

### Expected Result

- Search results satisfy all selected filter criteria.
- Only matching records are displayed.

---

## TC_ADMIN_USER_012 - Verify Reset Button Clears Search Filters

**Priority**

Medium

**Objective**

Verify that the Reset button clears all search criteria.

### Test Steps

| Step | Action |
|------|--------|
|1|Fill one or more search fields.|
|2|Click **Reset**.|

### Expected Result

- All search fields are cleared.
- Default values are restored.
- User list returns to its default state.

---

## TC_ADMIN_USER_013 - Search with Empty Filters

**Priority**

Medium

**Objective**

Verify that clicking Search without any filter displays all users.

### Test Steps

| Step | Action |
|------|--------|
|1|Leave all search fields empty.|
|2|Click **Search**.|

### Expected Result

- All available user records are displayed.
- No validation message is shown.

---

## TC_ADMIN_USER_014 - Add User with Valid Information

**Priority**

High

**Objective**

Verify that a new user can be successfully created using valid information.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Select User Role.|
|3|Select an existing Employee Name.|
|4|Select Status.|
|5|Enter a valid Username.|
|6|Enter Password.|
|7|Enter matching Confirm Password.|
|8|Click **Save**.|

### Expected Result

- New user is created successfully.
- Success toast notification is displayed.
- User appears in the User List.

---

## TC_ADMIN_USER_015 - Add User with Empty Required Fields

**Priority**

High

**Objective**

Verify that required field validation is displayed when mandatory fields are left empty.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Leave all required fields empty.|
|3|Click **Save**.|

### Expected Result

- Required validation messages are displayed.
- User is not created.

---

## TC_ADMIN_USER_016 - Verify Employee Name Autocomplete

**Priority**

High

**Objective**

Verify that Employee Name only accepts existing employees from autocomplete suggestions.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Type part of an existing employee name.|
|3|Observe autocomplete suggestions.|
|4|Select one suggestion.|

### Expected Result

- Matching employee suggestions are displayed.
- Selected employee is populated into the field.

---

## TC_ADMIN_USER_017 - Verify Invalid Employee Name Cannot Be Selected

**Priority**

High

**Objective**

Verify that arbitrary Employee Name values cannot be submitted.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Type a non-existing employee name.|
|3|Attempt to save without selecting an autocomplete suggestion.|

### Expected Result

- Validation message is displayed.
- User cannot be created.
- Employee Name field requires a valid existing employee.

---

## TC_ADMIN_USER_018 - Verify Username Minimum Length Validation

**Priority**

High

**Objective**

Verify that Username must contain at least five characters.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Complete all required fields.|
|3|Enter a Username containing fewer than five characters.|
|4|Click **Save**.|

### Expected Result

- Username validation message is displayed.
- User is not created.

---

## TC_ADMIN_USER_019 - Verify Password and Confirm Password Validation

**Priority**

High

**Objective**

Verify that Password and Confirm Password must match.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Complete all required fields.|
|3|Enter different values in Password and Confirm Password.|
|4|Click **Save**.|

### Expected Result

- Password mismatch validation is displayed.
- User is not created.

---

## TC_ADMIN_USER_020 - Cancel User Creation

**Priority**

Medium

**Objective**

Verify that clicking Cancel discards user creation.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Fill one or more fields.|
|3|Click **Cancel**.|

### Expected Result

- Add User page is closed.
- User Management page is displayed.
- No new user is created.

---

## TC_ADMIN_USER_021 - Edit Username Successfully

**Priority**

High

**Objective**

Verify that an administrator can successfully update a user's username.

### Test Steps

| Step | Action |
|------|--------|
|1|Select an existing user.|
|2|Click **Edit**.|
|3|Modify the Username.|
|4|Click **Save**.|

### Expected Result

- Username is successfully updated.
- Success toast notification is displayed.
- Updated username is displayed in the User List.

---

## TC_ADMIN_USER_022 - Edit User Role Successfully

**Priority**

High

**Objective**

Verify that User Role can be updated successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Change the User Role.|
|3|Click **Save**.|

### Expected Result

- User Role is updated successfully.
- Success toast notification is displayed.
- Updated User Role appears in the User List.

---

## TC_ADMIN_USER_023 - Edit Employee Name Successfully

**Priority**

High

**Objective**

Verify that Employee Name can be updated using autocomplete.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Enter a different Employee Name.|
|3|Select a suggestion from autocomplete.|
|4|Click **Save**.|

### Expected Result

- Employee Name is updated successfully.
- Success toast notification is displayed.
- Updated Employee Name appears in the User List.

---

## TC_ADMIN_USER_024 - Edit Status Successfully

**Priority**

High

**Objective**

Verify that user status can be updated.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Change Status.|
|3|Click **Save**.|

### Expected Result

- Status is updated successfully.
- Success toast notification is displayed.
- Updated Status appears in the User List.

---

## TC_ADMIN_USER_025 - Verify Change Password Checkbox

**Priority**

High

**Objective**

Verify that enabling Change Password displays Password and Confirm Password fields.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Tick the **Change Password** checkbox.|

### Expected Result

- Password field appears.
- Confirm Password field appears.
- Both fields are editable.

---

## TC_ADMIN_USER_026 - Change Password Successfully

**Priority**

High

**Objective**

Verify that a user's password can be updated successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Enable **Change Password**.|
|3|Enter a valid Password.|
|4|Enter the matching Confirm Password.|
|5|Click **Save**.|

### Expected Result

- Password is updated successfully.
- Success toast notification is displayed.

---

## TC_ADMIN_USER_027 - Verify Password Confirmation Validation During Edit

**Priority**

High

**Objective**

Verify that the system validates mismatched passwords during password update.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Enable **Change Password**.|
|3|Enter different values for Password and Confirm Password.|
|4|Click **Save**.|

### Expected Result

- Password mismatch validation message is displayed.
- Changes are not saved.

---

## TC_ADMIN_USER_028 - Verify Required Password Fields After Enabling Change Password

**Priority**

High

**Objective**

Verify that Password and Confirm Password become mandatory after enabling Change Password.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Enable **Change Password**.|
|3|Leave Password and Confirm Password empty.|
|4|Click **Save**.|

### Expected Result

- Required validation messages are displayed.
- User information is not updated.

---

## TC_ADMIN_USER_029 - Cancel User Update

**Priority**

Medium

**Objective**

Verify that clicking Cancel discards all modifications.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Modify one or more fields.|
|3|Click **Cancel**.|

### Expected Result

- Edit User page is closed.
- User Management page is displayed.
- No changes are saved.

---

## TC_ADMIN_USER_030 - Verify Success Toast After Updating User

**Priority**

Medium

**Objective**

Verify that a success notification is displayed after updating user information.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Edit User page.|
|2|Modify any editable field.|
|3|Click **Save**.|

### Expected Result

- Success toast notification is displayed.
- Updated information is saved successfully.

---

## TC_ADMIN_USER_031 - Delete User Successfully

**Priority**

High

**Objective**

Verify that an administrator can successfully delete an existing user.

### Test Steps

| Step | Action |
|------|--------|
|1|Open User Management page.|
|2|Click the **Delete** icon for an existing user.|
|3|Click **Yes, Delete** in the confirmation dialog.|

### Expected Result

- User is deleted successfully.
- Success toast notification is displayed.
- Deleted user no longer appears in the User List.

---

## TC_ADMIN_USER_032 - Cancel User Deletion

**Priority**

Medium

**Objective**

Verify that cancelling the delete confirmation does not remove the selected user.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Delete** icon for an existing user.|
|2|Click **No, Cancel**.|

### Expected Result

- Confirmation dialog is closed.
- User remains in the User List.
- No changes are made.

---

## TC_ADMIN_USER_033 - Verify Delete Confirmation Dialog

**Priority**

Medium

**Objective**

Verify that a confirmation dialog is displayed before deleting a user.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Delete** icon.|

### Expected Result

- Delete confirmation dialog is displayed.
- User cannot be deleted without confirmation.

---

## TC_ADMIN_USER_034 - Verify Username Column Sorting

**Priority**

Medium

**Objective**

Verify that the Username column can be sorted in ascending and descending order.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the Username column header.|
|2|Observe the displayed order.|
|3|Click the Username column header again.|

### Expected Result

- First click sorts usernames in ascending order.
- Second click sorts usernames in descending order.

---

## TC_ADMIN_USER_035 - Verify User Role Column Sorting

**Priority**

Medium

**Objective**

Verify that the User Role column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the User Role column header twice.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_ADMIN_USER_036 - Verify Employee Name Column Sorting

**Priority**

Medium

**Objective**

Verify that the Employee Name column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the Employee Name column header twice.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_ADMIN_USER_037 - Verify Status Column Sorting

**Priority**

Medium

**Objective**

Verify that the Status column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the Status column header twice.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_ADMIN_USER_038 - Verify Username with Minimum Allowed Length

**Priority**

High

**Objective**

Verify that the system accepts a username containing exactly five characters.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Complete all required fields.|
|3|Enter a username containing exactly five characters.|
|4|Click **Save**.|

### Expected Result

- User is created successfully.
- Success toast notification is displayed.

---

## TC_ADMIN_USER_039 - Verify Leading and Trailing Spaces in Username

**Priority**

Medium

**Objective**

Verify how the system handles leading and trailing spaces in the Username field.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Complete all required fields.|
|3|Enter a username containing leading and trailing spaces.|
|4|Click **Save**.|

### Expected Result

- Username is processed correctly according to the system's validation rules.
- No unexpected behavior occurs.

---

## TC_ADMIN_USER_040 - Verify Employee Name Only Accepts Existing Employees

**Priority**

High

**Objective**

Verify that the Employee Name field only accepts existing employees from the autocomplete list.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Type a random employee name that does not exist.|
|3|Attempt to save without selecting an autocomplete suggestion.|

### Expected Result

- Employee Name validation is displayed.
- User cannot be created.
- Only existing employees can be selected.

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| User List | ✅ |
| Search User | ✅ |
| Add User | ✅ |
| Edit User | ✅ |
| Delete User | ✅ |
| Sorting | ✅ |
| Username Validation | ✅ |
| Employee Name Validation | ✅ |
| Password Validation | ✅ |
| Toast Notification | ✅ |

---

# Notes

- These test cases verify the functional behavior of the **Admin → User Management** feature.
- Test execution results, evidence, and bug reports are documented separately in the **Test Execution** and **Bug Report** documents.
- Additional test cases may be added in the future as new functionality becomes available or new defects are identified during exploratory testing.
