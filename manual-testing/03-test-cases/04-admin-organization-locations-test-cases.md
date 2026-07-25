# Admin Organization Locations Test Cases

## Overview

This document contains the manual test cases for the **Locations** feature under the **Admin → Organization** module in the OrangeHRM Demo application.

The objective is to verify that users can manage organization locations correctly, including searching, creating, updating, deleting, validating inputs, and interacting with the data table.

---

# Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | Organization - Locations |
| Test Type | Functional Testing |
| Test Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

# Preconditions

Before executing the test cases, ensure that:

- OrangeHRM Demo website is accessible.
- User is logged in as Administrator.
- User has permission to access **Admin → Organization → Locations**.
- Internet connection is stable.

---

# Test Data

| Field | Sample Data |
|------|-------------|
| Name | Jakarta Office |
| City | Jakarta |
| State / Province | DKI Jakarta |
| Zip / Postal Code | 12345 |
| Country | Indonesia |
| Phone | +62-8123456789 |
| Fax | 021123456 |
| Address | Jl. Sudirman No.1 |
| Notes | Main office |

---

# Test Cases

---

## TC_LOC_001 - Verify Locations Page Loads Successfully

**Priority**

High

**Objective**

Verify that the Locations page can be opened successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Navigate to **Admin → Organization → Locations**.|

### Expected Result

- Locations page loads successfully.
- Locations table is displayed.
- Add button is visible.

---

## TC_LOC_002 - Verify Locations Table Structure

**Priority**

High

**Objective**

Verify that the Locations table displays all expected columns.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Locations page.|

### Expected Result

The table displays:

- Checkbox
- Name
- City
- Country
- Phone
- Number of Employees
- Actions

---

## TC_LOC_003 - Search Using Full Location Name

**Priority**

High

**Objective**

Verify that users can search by the complete Location Name.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter a complete Location Name in the Search field.|
|2|Click **Search**.|

### Expected Result

- Matching location is displayed.

---

## TC_LOC_004 - Search Using Partial Keyword

**Priority**

High

**Objective**

Verify that search supports partial keywords.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter part of a Location Name.|
|2|Click **Search**.|

### Expected Result

- Matching locations containing the keyword are displayed.

---

## TC_LOC_005 - Search Using City

**Priority**

Medium

**Objective**

Verify that users can search locations by City.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter a City name.|
|2|Click **Search**.|

### Expected Result

- Locations from the specified City are displayed.

---

## TC_LOC_006 - Search Using Country

**Priority**

Medium

**Objective**

Verify that users can search locations by Country.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter a Country name.|
|2|Click **Search**.|

### Expected Result

- Locations from the selected Country are displayed.

---

## TC_LOC_007 - Search with No Matching Result

**Priority**

Medium

**Objective**

Verify system behavior when no matching records exist.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter an invalid search keyword.|
|2|Click **Search**.|

### Expected Result

- No matching records are displayed.
- Empty result message is shown.

---

## TC_LOC_008 - Open Add Location Form

**Priority**

High

**Objective**

Verify that the Add Location form opens successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|

### Expected Result

- Add Location form is displayed.

---

## TC_LOC_009 - Add Location with Valid Data

**Priority**

High

**Objective**

Verify that a new Location can be created successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Fill all required fields with valid data.|
|3|Click **Save**.|

### Expected Result

- New Location is created successfully.
- Success toast notification is displayed.
- Record appears in the table.

---

## TC_LOC_010 - Add Location Using Only Required Fields

**Priority**

Medium

**Objective**

Verify that only required fields are needed to create a Location.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Fill only Name and Country.|
|3|Click **Save**.|

### Expected Result

- Location is created successfully.
- Optional fields remain empty.

---

## TC_LOC_011 - Verify Required Validation for Location Name

**Priority**

High

**Objective**

Verify that the Name field is mandatory.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Leave the Name field empty.|
|3|Select a Country.|
|4|Click **Save**.|

### Expected Result

- **"Required"** validation message is displayed below the Name field.
- Location is not created.

---

## TC_LOC_012 - Verify Required Validation for Country

**Priority**

High

**Objective**

Verify that the Country field is mandatory.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Name.|
|3|Leave Country empty.|
|4|Click **Save**.|

### Expected Result

- **"Required"** validation message is displayed below the Country field.
- Location is not created.

---

## TC_LOC_013 - Verify Duplicate Location Name Validation

**Priority**

High

**Objective**

Verify that duplicate Location Names cannot be created.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter an existing Location Name.|
|3|Select any Country.|
|4|Click **Save**.|

### Expected Result

- Duplicate validation message is displayed.
- New Location is not created.

---

## TC_LOC_014 - Verify Country Dropdown Selection

**Priority**

Medium

**Objective**

Verify that users can select a Country from the dropdown list.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Open the Country dropdown.|
|3|Select any Country.|

### Expected Result

- Selected Country is displayed in the Country field.

---

## TC_LOC_015 - Verify Country Selection Using Keyboard

**Priority**

Medium

**Objective**

Verify that users can quickly select a Country using keyboard input.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Country dropdown.|
|2|Type the first few letters of a Country name.|
|3|Select the highlighted Country.|

### Expected Result

- Matching Country is highlighted.
- Selected Country is displayed correctly.

---

## TC_LOC_016 - Open Edit Location Form

**Priority**

High

**Objective**

Verify that the Edit Location form opens successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Edit** button for an existing Location.|

### Expected Result

- Edit Location form is displayed.
- Existing data is pre-filled.

---

## TC_LOC_017 - Update Location with Valid Data

**Priority**

High

**Objective**

Verify that Location information can be updated successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Modify one or more fields.|
|3|Click **Save**.|

### Expected Result

- Location is updated successfully.
- Success toast notification is displayed.
- Updated information appears in the table.

---

## TC_LOC_018 - Update Only One Field

**Priority**

Medium

**Objective**

Verify that users can update only one field without changing the others.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Modify only one field (e.g., City).|
|3|Click **Save**.|

### Expected Result

- Modified field is updated successfully.
- Other fields remain unchanged.

---

## TC_LOC_019 - Verify Required Validation During Edit

**Priority**

High

**Objective**

Verify that required validation is enforced during editing.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Clear the Name field.|
|3|Click **Save**.|

### Expected Result

- **"Required"** validation message is displayed.
- Changes are not saved.

---

## TC_LOC_020 - Cancel Edit Location

**Priority**

Medium

**Objective**

Verify that cancelling an edit discards all changes.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Modify one or more fields.|
|3|Click **Cancel**.|

### Expected Result

- Edit form is closed.
- No changes are saved.
- Original data remains unchanged.

---

## TC_LOC_021 - Delete Location Successfully

**Priority**

High

**Objective**

Verify that an existing Location can be deleted successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Select an existing Location.|
|2|Click **Delete**.|
|3|Confirm the deletion.|

### Expected Result

- Selected Location is deleted successfully.
- Success toast notification is displayed.
- Record is removed from the table.

---

## TC_LOC_022 - Cancel Delete Location

**Priority**

Medium

**Objective**

Verify that Location deletion is cancelled successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Select an existing Location.|
|2|Click **Delete**.|
|3|Click **Cancel** on the confirmation dialog.|

### Expected Result

- Confirmation dialog is closed.
- No records are deleted.
- Selected Location remains in the table.

---

## TC_LOC_023 - Delete Multiple Locations

**Priority**

High

**Objective**

Verify that multiple Locations can be deleted simultaneously.

### Test Steps

| Step | Action |
|------|--------|
|1|Select multiple Locations using the checkboxes.|
|2|Click **Delete Selected**.|
|3|Confirm the deletion.|

### Expected Result

- All selected Locations are deleted successfully.
- Success toast notification is displayed.
- Selected records are removed from the table.

---

## TC_LOC_024 - Verify Select All Checkbox

**Priority**

Medium

**Objective**

Verify that the Select All checkbox selects all available records.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Select All** checkbox.|

### Expected Result

- All rows are selected.
- Individual checkboxes are checked.
- Bulk Delete action becomes available.

---

## TC_LOC_025 - Verify Individual Row Selection

**Priority**

Low

**Objective**

Verify that users can select individual rows.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the checkbox of a single Location.|

### Expected Result

- Selected row is checked.
- Bulk Delete action becomes available.

---

## TC_LOC_026 - Verify Sorting by Name

**Priority**

Medium

**Objective**

Verify that the Name column supports ascending and descending sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Name** column header.|
|2|Click it again.|

### Expected Result

- Records are sorted in ascending order.
- Clicking again sorts records in descending order.

---

## TC_LOC_027 - Verify Sorting by City

**Priority**

Medium

**Objective**

Verify that the City column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **City** column header.|
|2|Click it again.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_LOC_028 - Verify Sorting by Country

**Priority**

Medium

**Objective**

Verify that the Country column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Country** column header.|
|2|Click it again.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_LOC_029 - Verify Sorting by Phone

**Priority**

Low

**Objective**

Verify that the Phone column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Phone** column header.|
|2|Click it again.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_LOC_030 - Verify Sorting by Number of Employees

**Priority**

Low

**Objective**

Verify that the Number of Employees column supports sorting.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Number of Employees** column header.|
|2|Click it again.|

### Expected Result

- Records are sorted correctly in ascending and descending order.

---

## TC_LOC_031 - Verify Phone Field Accepts Valid Characters

**Priority**

Medium

**Objective**

Verify that the Phone field accepts valid phone number characters.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Name and Country.|
|3|Enter a phone number containing digits and supported symbols (e.g., +62-8123456789 or (021)123456).|
|4|Click **Save**.|

### Expected Result

- Phone number is accepted.
- Location is created successfully.

---

## TC_LOC_032 - Verify Phone Field Rejects Alphabetic Characters

**Priority**

Medium

**Objective**

Verify that the Phone field rejects alphabetic characters.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter valid required fields.|
|3|Enter alphabetic characters in the Phone field (e.g., abcdef).|
|4|Click **Save**.|

### Expected Result

- Phone field validation is triggered.
- Location is not created until a valid phone number is entered.

---

## TC_LOC_033 - Verify Zip / Postal Code Accepts Numeric Value

**Priority**

Low

**Objective**

Verify that the Zip / Postal Code field accepts numeric values.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter valid required fields.|
|3|Enter a numeric Zip / Postal Code.|
|4|Click **Save**.|

### Expected Result

- Numeric Zip / Postal Code is accepted.
- Location is created successfully.

---

## TC_LOC_034 - Verify Zip / Postal Code Accepts Alphanumeric Value

**Priority**

Low

**Objective**

Verify that the Zip / Postal Code field accepts alphanumeric values.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter valid required fields.|
|3|Enter an alphanumeric Zip / Postal Code (e.g., AB123).|
|4|Click **Save**.|

### Expected Result

- Alphanumeric Zip / Postal Code is accepted.
- Location is created successfully.

---

## TC_LOC_035 - Verify Zip / Postal Code Accepts Special Characters

**Priority**

Low

**Objective**

Verify that the Zip / Postal Code field accepts special characters.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter valid required fields.|
|3|Enter special characters in the Zip / Postal Code field.|
|4|Click **Save**.|

### Expected Result

- Special characters are accepted.
- Location is created successfully.

---

## TC_LOC_036 - Verify Success Toast Notification

**Priority**

Low

**Objective**

Verify that a success toast notification is displayed after a successful Add, Edit, or Delete operation.

### Test Steps

| Step | Action |
|------|--------|
|1|Perform a successful Add, Edit, or Delete operation.|

### Expected Result

- Success toast notification is displayed.
- Notification disappears automatically after a short period.

---

## TC_LOC_037 - Verify Total Records After CRUD Operations

**Priority**

Low

**Objective**

Verify that the total record count is updated after creating or deleting a Location.

### Test Steps

| Step | Action |
|------|--------|
|1|Record the current total number of Locations.|
|2|Add a new Location.|
|3|Delete the newly created Location.|

### Expected Result

- Total records increase after adding a Location.
- Total records decrease after deleting the Location.

---

## TC_LOC_038 - Verify Existing Data Is Pre-filled During Edit

**Priority**

Medium

**Objective**

Verify that all existing Location information is automatically populated when opening the Edit form.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Edit** on an existing Location.|

### Expected Result

- All existing values are automatically populated in their respective fields.
- User can modify only the desired fields without re-entering all information.

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| Page Navigation | ✅ |
| Table Display | ✅ |
| Search | ✅ |
| Add Location | ✅ |
| Edit Location | ✅ |
| Delete Location | ✅ |
| Multiple Delete | ✅ |
| Select All | ✅ |
| Required Validation | ✅ |
| Duplicate Validation | ✅ |
| Country Selection | ✅ |
| Phone Validation | ✅ |
| Zip / Postal Code Validation | ✅ |
| Sorting | ✅ |
| Toast Notification | ✅ |
| Total Records | ✅ |

---

# Notes

- These test cases define the expected behavior of the **Admin → Organization → Locations** feature.
- Test execution results, evidence, and bug reports are documented separately in the **Test Execution** and **Bug Report** folders.
- Additional exploratory testing may reveal usability issues or unexpected behaviors that are not covered by these predefined test cases.
