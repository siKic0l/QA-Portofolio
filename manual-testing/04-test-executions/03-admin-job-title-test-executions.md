# Admin Job Title Test Execution

## Overview

This document records the execution results of all manual test cases for the **Job Titles** feature under the **Admin** module in the OrangeHRM Demo application.

The purpose of this document is to track execution progress, record actual results, provide execution evidence, and document any defects identified during testing.

---

# Execution Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | Job Titles |
| Test Type | Manual Functional Testing |
| Tester | Nurrohmi Zaki |
| Environment | Windows 11 • Google Chrome (Latest) |
| Execution Date | *To be updated* |
| Execution Status | Completed |

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_ADMIN_JOB_001 | Verify Job Titles page loads successfully | Job Titles page loads successfully. | Job Titles page loaded successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_001_PASS.png) | - |
| TC_ADMIN_JOB_002 | Verify Job Titles table structure | Table and columns are displayed correctly. | Table and columns were displayed correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_002_PASS.png) | - |
| TC_ADMIN_JOB_003 | Verify Add button | Add Job Title form is displayed. | Add Job Title form was displayed successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_003_PASS.png) | - |
| TC_ADMIN_JOB_004 | Verify Edit button | Edit Job Title form is displayed. | Edit Job Title form was displayed successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_004_PASS.png) | - |
| TC_ADMIN_JOB_005 | Verify Delete button | Delete confirmation dialog is displayed. | Delete confirmation dialog was displayed successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_005_PASS.png) | - |
| TC_ADMIN_JOB_006 | Add Job Title with valid data | New Job Title is created successfully. | New Job Title was created successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_006_PASS.png) | - |
| TC_ADMIN_JOB_007 | Verify required validation for Job Title | Required validation message is displayed. | Required validation message was displayed correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_007_PASS.png) | - |
| TC_ADMIN_JOB_008 | Verify duplicate Job Title validation | Duplicate Job Title is rejected. | Duplicate Job Title was rejected successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_008_PASS.png) | - |
| TC_ADMIN_JOB_009 | Add Job Title without Description | Job Title is created successfully. | Job Title was created successfully without Description. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_009_PASS.png) | - |
| TC_ADMIN_JOB_010 | Add Job Title without Notes | Job Title is created successfully. | Job Title was created successfully without Notes. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_010_PASS.png) | - |
| TC_ADMIN_JOB_011 | Add Job Title without optional fields | Job Title is created successfully. | Job Title was created successfully using only required fields. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_011_PASS.png) | - |
| TC_ADMIN_JOB_012 | Upload supported image file | Supported file is uploaded successfully. | Supported image file was uploaded successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_012_PASS.png) | - |
| TC_ADMIN_JOB_013 | Upload unsupported file type | Unsupported file is rejected. | Unsupported file type was rejected successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_013_PASS.png) | - |
| TC_ADMIN_JOB_014 | Cancel Add Job Title | Add operation is cancelled without saving data. | Add operation was cancelled successfully without saving data. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_014_PASS.png) | - |
| TC_ADMIN_JOB_015 | Edit Job Title successfully | Job Title is updated successfully. | Job Title was updated successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_015_PASS.png) | - |
| TC_ADMIN_JOB_016 | Edit Job Description | Job Description is updated successfully. | Job Description was updated successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_016_PASS.png) | - |
| TC_ADMIN_JOB_017 | Edit Notes | Notes are updated successfully. | Notes were updated successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_017_PASS.png) | - |
| TC_ADMIN_JOB_018 | Replace uploaded specification file | Uploaded file is replaced successfully. | Uploaded specification file was replaced successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_018_PASS.png) | - |
| TC_ADMIN_JOB_019 | Edit Job Title to duplicate name | Duplicate validation message is displayed. | Duplicate validation message was displayed correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_019_PASS.png) | - |
| TC_ADMIN_JOB_020 | Cancel Job Title update | Changes are discarded successfully. | Changes were discarded successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_020_PASS.png) | - |
| TC_ADMIN_JOB_021 | Verify success toast after updating Job Title | Success toast notification is displayed. | Success toast notification was displayed correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_021_PASS.png) | - |
| TC_ADMIN_JOB_022 | Delete a Job Title successfully | Selected Job Title is deleted successfully. | Selected Job Title was deleted successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_022_PASS.png) | - |
| TC_ADMIN_JOB_023 | Cancel Job Title deletion | Deletion is cancelled successfully. | Deletion was cancelled successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_023_PASS.png) | - |
| TC_ADMIN_JOB_024 | Delete multiple Job Titles | Selected Job Titles are deleted successfully. | Selected Job Titles were deleted successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_024_PASS.png) | - |
| TC_ADMIN_JOB_025 | Select All Job Titles | All rows are selected successfully. | All rows were selected successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_025_PASS.png) | - |
| TC_ADMIN_JOB_026 | Verify success toast after deletion | Success toast notification is displayed. | Success toast notification was displayed correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_026_PASS.png) | - |
| TC_ADMIN_JOB_027 | Verify Job Title sorting (Ascending) | Job Titles are sorted in ascending order. | Job Titles were sorted in ascending order correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_027_PASS.png) | - |
| TC_ADMIN_JOB_028 | Verify Job Title sorting (Descending) | Job Titles are sorted in descending order. | Job Titles were sorted in descending order correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_028_PASS.png) | - |
| TC_ADMIN_JOB_029 | Verify checkbox selection | Checkbox selection works correctly. | Checkbox selection worked correctly. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_029_PASS.png) | - |
| TC_ADMIN_JOB_030 | Verify total record count after adding a Job Title | Total record count increases by one. | Total record count increased correctly after adding a Job Title. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_030_PASS.png) | - |
| TC_ADMIN_JOB_031 | Verify total record count after deleting a Job Title | Total record count decreases by one. | Total record count decreased correctly after deleting a Job Title. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_031_PASS.png) | - |
| TC_ADMIN_JOB_032 | Upload JPG/JPEG image as Job Specification | JPG/JPEG image is uploaded successfully. | JPG/JPEG image was uploaded successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_032_PASS.png) | - |
| TC_ADMIN_JOB_033 | Upload PNG image as Job Specification | PNG image is uploaded successfully. | PNG image was uploaded successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_033_PASS.png) | - |
| TC_ADMIN_JOB_034 | Verify Job Title uniqueness | Duplicate Job Title cannot be created. | Duplicate Job Title could not be created. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_034_PASS.png) | - |
| TC_ADMIN_JOB_035 | Verify Job Specification file size limit | Files larger than 1 MB are rejected. | Files larger than 1 MB were rejected successfully. | ✅ PASS | [View Evidence](../evidence/Admin-Job-Title/TC_ADMIN_JOB_035_PASS.png) | - |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 35 |
| Passed | 35 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 0 |
| Pass Rate | 100% |

---

# Notes

- All planned test cases were executed successfully.
- No functional defects were identified during test execution.
- All supporting evidence is available in the **evidence/Admin-Job-Title/** directory.
- Additional exploratory testing was performed, but no functional defects were identified.
