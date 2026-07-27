# Admin Job Title Test Scenarios

## Overview

This document defines the manual test scenarios for the **Job Titles** feature under the **Admin** module in the OrangeHRM Demo application.

The objective is to verify that users can manage Job Titles correctly, including creating, editing, deleting, uploading job specifications, validating input, and interacting with the table.

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

Before executing the test scenarios, ensure that:

- OrangeHRM Demo website is accessible.
- User is logged in as Administrator.
- User has permission to access **Admin → Job → Job Titles**.
- At least one Job Title record exists for edit and delete scenarios.

---

# Test Scenarios

| Scenario ID | Scenario | Priority |
|-------------|----------|----------|
| TS_ADMIN_JOB_001 | Verify Job Titles page loads successfully | High |
| TS_ADMIN_JOB_002 | Verify Job Titles table displays correctly | High |
| TS_ADMIN_JOB_003 | Verify Add button opens the Add Job Title form | High |
| TS_ADMIN_JOB_004 | Verify Edit button opens the Edit Job Title form | High |
| TS_ADMIN_JOB_005 | Verify Delete button opens the confirmation dialog | High |
| TS_ADMIN_JOB_006 | Verify a new Job Title can be added successfully | High |
| TS_ADMIN_JOB_007 | Verify Job Title is a required field | High |
| TS_ADMIN_JOB_008 | Verify duplicate Job Title is not allowed | High |
| TS_ADMIN_JOB_009 | Verify Job Description field is optional | Medium |
| TS_ADMIN_JOB_010 | Verify Notes field is optional | Medium |
| TS_ADMIN_JOB_011 | Verify supported specification files can be uploaded | Medium |
| TS_ADMIN_JOB_012 | Verify unsupported file types are rejected | High |
| TS_ADMIN_JOB_013 | Verify uploaded specification file can be replaced during edit | Medium |
| TS_ADMIN_JOB_014 | Verify Job Title information can be edited successfully | High |
| TS_ADMIN_JOB_015 | Verify Cancel button discards changes | Medium |
| TS_ADMIN_JOB_016 | Verify a single Job Title can be deleted | High |
| TS_ADMIN_JOB_017 | Verify multiple Job Titles can be deleted | High |
| TS_ADMIN_JOB_018 | Verify Select All checkbox functionality | Medium |
| TS_ADMIN_JOB_019 | Verify Job Title sorting in ascending and descending order | Medium |
| TS_ADMIN_JOB_020 | Verify total record count updates after Add and Delete operations | Medium |

---

# Test Coverage

| Feature | Coverage |
|----------|----------|
| Page Navigation | Yes |
| Table Display | Yes |
| Add Job Title | Yes |
| Edit Job Title | Yes |
| Delete Job Title | Yes |
| Multiple Delete | Yes |
| Select All | Yes |
| Required Validation | Yes |
| Duplicate Validation | Yes |
| File Upload | Yes |
| File Type Validation | Yes |
| Sorting | Yes |
| Toast Notification | Yes |
| Total Records | Yes |

---

# Notes

- These scenarios define the functional behaviors that will be verified during manual testing.
- Detailed execution steps are documented separately in the **Admin Job Title Test Cases** document.
- Test execution results, evidence, and bug reports will be documented in the corresponding **Test Execution** and **Bug Report** documents.
