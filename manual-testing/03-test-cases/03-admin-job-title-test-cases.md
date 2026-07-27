# Admin Job Title Test Cases

## Overview

This document contains the manual test cases for the **Job Titles** feature under the **Admin** module in the OrangeHRM Demo application.

The objective is to verify that administrators can manage Job Titles correctly, including creating, editing, deleting, uploading job specifications, validating input, and interacting with the Job Titles table.

---

# Module Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | Job Titles |
| Test Type | Functional Testing |
| Test Technique | Black Box Testing |
| Tester | Nurrohmi Zaki |

---

# Preconditions

Before executing the test cases, ensure that:

- OrangeHRM Demo website is accessible.
- User is logged in as Administrator.
- User has permission to access **Admin → Job → Job Titles**.
- At least one Job Title exists for edit and delete scenarios.

---

# Test Data

| Job Title | Description | Specification | Notes | Purpose |
|-----------|-------------|---------------|-------|----------|
| QA Engineer | Manual testing activities | qa-spec.pdf | QA Team | Valid data |
| Software Engineer | Software development | developer.pdf | IT Team | Valid data |
| QA Engineer | Duplicate title | qa-spec.pdf | Duplicate | Duplicate validation |
| *(empty)* | Any | Any | Any | Required validation |
| Video File | Sample | sample.mp4 | Invalid | Unsupported file |
| Large File | Sample | specification_1_5MB.pdf | Boundary | File size validation |

---

# Test Cases

---

## TC_ADMIN_JOB_001 - Verify Job Titles Page Loads Successfully

**Priority**

High

**Objective**

Verify that the Job Titles page loads correctly.

### Test Steps

| Step | Action |
|------|--------|
|1|Navigate to **Admin → Job → Job Titles**.|

### Expected Result

- Job Titles page is displayed successfully.
- Table is visible.
- Action buttons are available.

---

## TC_ADMIN_JOB_002 - Verify Job Titles Table Structure

**Priority**

High

**Objective**

Verify that the Job Titles table displays correctly.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Job Titles page.|

### Expected Result

- Table is displayed.
- Columns are displayed correctly:
  - Checkbox
  - Job Title
  - Job Description
  - Actions

---

## TC_ADMIN_JOB_003 - Verify Add Button

**Priority**

High

**Objective**

Verify that the Add button opens the Add Job Title form.

### Test Steps

| Step | Action |
|------|--------|
|1|Open Job Titles page.|
|2|Click **Add**.|

### Expected Result

- Add Job Title form is displayed.

---

## TC_ADMIN_JOB_004 - Verify Edit Button

**Priority**

High

**Objective**

Verify that the Edit button opens the Edit Job Title form.

### Test Steps

| Step | Action |
|------|--------|
|1|Select any Job Title.|
|2|Click **Edit**.|

### Expected Result

- Edit Job Title form is displayed.

---

## TC_ADMIN_JOB_005 - Verify Delete Button

**Priority**

High

**Objective**

Verify that the Delete button opens the confirmation dialog.

### Test Steps

| Step | Action |
|------|--------|
|1|Select any Job Title.|
|2|Click **Delete**.|

### Expected Result

- Delete confirmation dialog is displayed.

---

## TC_ADMIN_JOB_006 - Add Job Title with Valid Data

**Priority**

High

**Objective**

Verify that a new Job Title can be created successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a unique Job Title.|
|3|Fill optional fields if needed.|
|4|Click **Save**.|

### Expected Result

- Job Title is created successfully.
- Success toast notification is displayed.
- New record appears in the table.

---

## TC_ADMIN_JOB_007 - Verify Required Validation for Job Title

**Priority**

High

**Objective**

Verify that Job Title is required.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Leave Job Title empty.|
|3|Click **Save**.|

### Expected Result

- Required validation message is displayed.
- Record is not created.

---

## TC_ADMIN_JOB_008 - Verify Duplicate Job Title Validation

**Priority**

High

**Objective**

Verify that duplicate Job Titles cannot be created.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter an existing Job Title.|
|3|Click **Save**.|

### Expected Result

- Duplicate validation message is displayed.
- Record is not created.

---

## TC_ADMIN_JOB_009 - Add Job Title Without Description

**Priority**

Medium

**Objective**

Verify that Job Description is optional.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter Job Title.|
|2|Leave Description empty.|
|3|Click **Save**.|

### Expected Result

- Record is created successfully.

---

## TC_ADMIN_JOB_010 - Add Job Title Without Notes

**Priority**

Medium

**Objective**

Verify that Notes field is optional.

### Test Steps

| Step | Action |
|------|--------|
|1|Enter Job Title.|
|2|Leave Notes empty.|
|3|Click **Save**.|

### Expected Result

- Record is created successfully.

---

## TC_ADMIN_JOB_011 - Add Job Title Without Optional Fields

**Priority**

Medium

**Objective**

Verify that a Job Title can be created by providing only the required field.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a unique Job Title.|
|3|Leave Job Description, Job Specification, and Notes empty.|
|4|Click **Save**.|

### Expected Result

- Job Title is created successfully.
- Success toast notification is displayed.
- New record appears in the table.

---

## TC_ADMIN_JOB_012 - Upload Supported Image File

**Priority**

Medium

**Objective**

Verify that supported image files can be uploaded successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload a supported image file (.jpg, .jpeg, or .png).|
|4|Click **Save**.|

### Expected Result

- File is uploaded successfully.
- Job Title is created successfully.

---

## TC_ADMIN_JOB_013 - Upload Unsupported File Type

**Priority**

High

**Objective**

Verify that unsupported file types cannot be uploaded.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload an unsupported file (e.g., .mp4 or .html).|
|4|Click **Save**.|

### Expected Result

- Upload is rejected.
- Appropriate validation message is displayed.
- Job Title is not created.

---

## TC_ADMIN_JOB_014 - Upload File Larger Than Documented Limit

**Priority**

Medium

**Objective**

Verify that files larger than the documented maximum size cannot be uploaded.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload a file larger than 1 MB.|
|4|Click **Save**.|

### Expected Result

- Upload is rejected.
- File size validation message is displayed.
- Job Title is not created.

---

## TC_ADMIN_JOB_015 - Cancel Add Job Title

**Priority**

Medium

**Objective**

Verify that clicking Cancel discards the new Job Title.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter Job Title information.|
|3|Click **Cancel**.|

### Expected Result

- Add form is closed.
- No new Job Title is created.

---

## TC_ADMIN_JOB_016 - Edit Job Title Successfully

**Priority**

High

**Objective**

Verify that an existing Job Title can be edited successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Select an existing Job Title.|
|2|Click **Edit**.|
|3|Modify the Job Title.|
|4|Click **Save**.|

### Expected Result

- Job Title is updated successfully.
- Success toast notification is displayed.
- Updated information is shown in the table.

---

## TC_ADMIN_JOB_017 - Edit Job Description

**Priority**

Medium

**Objective**

Verify that Job Description can be updated.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Modify Job Description.|
|3|Click **Save**.|

### Expected Result

- Job Description is updated successfully.

---

## TC_ADMIN_JOB_018 - Edit Notes

**Priority**

Medium

**Objective**

Verify that Notes can be updated successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Modify Notes.|
|3|Click **Save**.|

### Expected Result

- Notes are updated successfully.

---

## TC_ADMIN_JOB_019 - Replace Uploaded Specification File

**Priority**

Medium

**Objective**

Verify that the uploaded Job Specification file can be replaced.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Upload a different supported file.|
|3|Click **Save**.|

### Expected Result

- Previous file is replaced.
- Updated file is saved successfully.

---

## TC_ADMIN_JOB_020 - Edit Job Title to Duplicate Name

**Priority**

High

**Objective**

Verify that duplicate Job Titles are not allowed during editing.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit form.|
|2|Change the Job Title to an existing Job Title.|
|3|Click **Save**.|

### Expected Result

- Duplicate validation message is displayed.
- Changes are not saved.

---

## TC_ADMIN_JOB_021 - Cancel Job Title Update

**Priority**

Medium

**Objective**

Verify that clicking **Cancel** during editing discards all changes.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Edit Job Title form.|
|2|Modify one or more fields.|
|3|Click **Cancel**.|

### Expected Result

- Edit form is closed.
- No changes are saved.
- Original Job Title information remains unchanged.

---

## TC_ADMIN_JOB_022 - Verify Success Toast After Updating Job Title

**Priority**

Medium

**Objective**

Verify that a success notification is displayed after updating a Job Title.

### Test Steps

| Step | Action |
|------|--------|
|1|Edit an existing Job Title.|
|2|Click **Save**.|

### Expected Result

- Success toast notification is displayed.
- Updated information is reflected in the table.

---

## TC_ADMIN_JOB_023 - Delete a Job Title Successfully

**Priority**

High

**Objective**

Verify that a Job Title can be deleted successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Select a Job Title.|
|2|Click **Delete**.|
|3|Confirm the deletion.|

### Expected Result

- Selected Job Title is deleted successfully.
- Success toast notification is displayed.
- Record is removed from the table.

---

## TC_ADMIN_JOB_024 - Cancel Job Title Deletion

**Priority**

Medium

**Objective**

Verify that deletion is cancelled when the user selects **Cancel**.

### Test Steps

| Step | Action |
|------|--------|
|1|Select a Job Title.|
|2|Click **Delete**.|
|3|Click **Cancel** on the confirmation dialog.|

### Expected Result

- Confirmation dialog is closed.
- No records are deleted.
- Selected Job Title remains in the table.

---

## TC_ADMIN_JOB_025 - Delete Multiple Job Titles

**Priority**

High

**Objective**

Verify that multiple selected Job Titles can be deleted successfully.

### Test Steps

| Step | Action |
|------|--------|
|1|Select multiple Job Titles using the checkboxes.|
|2|Click **Delete Selected**.|
|3|Confirm the deletion.|

### Expected Result

- All selected Job Titles are deleted successfully.
- Success toast notification is displayed.
- Selected records are removed from the table.

---

## TC_ADMIN_JOB_026 - Select All Job Titles

**Priority**

Medium

**Objective**

Verify that the **Select All** checkbox selects every Job Title in the table.

### Test Steps

| Step | Action |
|------|--------|
|1|Open the Job Titles page.|
|2|Click the **Select All** checkbox.|

### Expected Result

- All rows are selected.
- Individual checkboxes are checked.
- Bulk Delete action becomes available.

---

## TC_ADMIN_JOB_027 - Verify Success Toast After Deletion

**Priority**

Medium

**Objective**

Verify that a success notification appears after deleting a Job Title.

### Test Steps

| Step | Action |
|------|--------|
|1|Delete an existing Job Title.|
|2|Confirm the deletion.|

### Expected Result

- Success toast notification is displayed.
- Deleted record no longer appears in the table.

---

## TC_ADMIN_JOB_028 - Verify Job Title Sorting (Ascending)

**Priority**

Medium

**Objective**

Verify that the Job Title column can be sorted in ascending order.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Job Title** column header.|

### Expected Result

- Job Titles are sorted alphabetically in ascending order (A–Z).

---

## TC_ADMIN_JOB_029 - Verify Job Title Sorting (Descending)

**Priority**

Medium

**Objective**

Verify that the Job Title column can be sorted in descending order.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the **Job Title** column header again.|

### Expected Result

- Job Titles are sorted alphabetically in descending order (Z–A).

---

## TC_ADMIN_JOB_030 - Verify Checkbox Selection

**Priority**

Low

**Objective**

Verify that individual Job Titles can be selected using the checkbox.

### Test Steps

| Step | Action |
|------|--------|
|1|Click the checkbox of a Job Title.|

### Expected Result

- Selected row is checked.
- Bulk Delete action becomes available.

---

## TC_ADMIN_JOB_031 - Verify Total Record Count After Adding a Job Title

**Priority**

Low

**Objective**

Verify that the total record count is updated after a new Job Title is added.

### Test Steps

| Step | Action |
|------|--------|
|1|Note the current total number of records.|
|2|Add a new Job Title.|
|3|Return to the Job Titles table.|

### Expected Result

- Total record count increases by one.
- Newly added Job Title appears in the table.

---

## TC_ADMIN_JOB_032 - Verify Total Record Count After Deleting a Job Title

**Priority**

Low

**Objective**

Verify that the total record count is updated after deleting a Job Title.

### Test Steps

| Step | Action |
|------|--------|
|1|Note the current total number of records.|
|2|Delete an existing Job Title.|
|3|Return to the Job Titles table.|

### Expected Result

- Total record count decreases by one.
- Deleted Job Title no longer appears in the table.

---

## TC_ADMIN_JOB_033 - Upload JPG/JPEG Image as Job Specification

**Priority**

Medium

**Objective**

Verify that JPG/JPEG image files can be uploaded successfully as Job Specification.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload a JPG or JPEG image.|
|4|Click **Save**.|

### Expected Result

- Image is uploaded successfully.
- Job Title is created successfully.

---

## TC_ADMIN_JOB_034 - Upload PNG Image as Job Specification

**Priority**

Medium

**Objective**

Verify that PNG image files can be uploaded successfully as Job Specification.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload a PNG image.|
|4|Click **Save**.|

### Expected Result

- Image is uploaded successfully.
- Job Title is created successfully.

---

## TC_ADMIN_JOB_035 - Verify Job Title Uniqueness

**Priority**

High

**Objective**

Verify that each Job Title must be unique.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter an existing Job Title.|
|3|Click **Save**.|

### Expected Result

- Duplicate validation message is displayed.
- Duplicate record is not created.

---

## TC_ADMIN_JOB_036 - Verify Job Specification File Size Limit

**Priority**

Medium

**Objective**

Verify that uploaded Job Specification files comply with the documented maximum file size.

### Test Steps

| Step | Action |
|------|--------|
|1|Click **Add**.|
|2|Enter a valid Job Title.|
|3|Upload a Job Specification file larger than **100 MB**.|
|4|Click **Save**.|

### Expected Result

- System accept files larger than **100 MB**.
- Appropriate validation message is displayed.
- Job Title is not created.

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| Page Navigation | ✅ |
| Table Display | ✅ |
| Add Job Title | ✅ |
| Edit Job Title | ✅ |
| Delete Job Title | ✅ |
| Multiple Delete | ✅ |
| Select All | ✅ |
| Required Validation | ✅ |
| Duplicate Validation | ✅ |
| File Upload | ✅ |
| File Type Validation | ✅ |
| File Size Validation | ✅ |
| Sorting | ✅ |
| Toast Notification | ✅ |
| Total Records | ✅ |

---

# Notes

- These test cases define the expected behavior of the **Admin → Job Titles** feature.
- Test execution results, evidence, and bug reports are documented separately in the **Test Execution** and **Bug Report** documents.
- Additional exploratory testing may identify usability issues or unexpected system behavior that are not covered by these predefined test cases.
