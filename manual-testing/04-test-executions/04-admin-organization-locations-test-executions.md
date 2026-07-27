# Admin Organization Locations Test Execution

## Overview

This document records the execution results of all manual test cases for the **Locations** feature under the **Admin → Organization** module in the OrangeHRM Demo application.

The purpose of this document is to track execution progress, record actual results, provide execution evidence, and link identified defects to the corresponding bug reports.

---

# Execution Information

| Item | Value |
|------|-------|
| Application | OrangeHRM Demo |
| Module | Admin |
| Feature | Organization - Locations |
| Test Type | Manual Functional Testing |
| Tester | Nurrohmi Zaki |
| Environment | Windows 11 • Google Chrome (Latest) |
| Execution Date | *To be updated* |
| Execution Status | Not Started |

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_ADMIN_LOC_001 | Verify Locations page loads successfully | Locations page loads successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_002 | Verify Locations table structure | Locations table displays all expected columns. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_003 | Search using full Location Name | Matching location is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_004 | Search using partial keyword | Matching locations are displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_005 | Search using City | Locations from the specified City are displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_006 | Search using Country | Locations from the specified Country are displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_007 | Search with no matching result | No matching records are displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_008 | Open Add Location form | Add Location form is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_009 | Add Location with valid data | Location is created successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_010 | Add Location using only required fields | Location is created successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_011 | Verify required validation for Location Name | Required validation message is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_012 | Verify required validation for Country | Required validation message is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_013 | Verify duplicate Location Name validation | Duplicate Location Name is rejected. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_014 | Verify Country dropdown selection | Country is selected successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_015 | Verify Country selection using keyboard | Country is selected using keyboard navigation. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_016 | Open Edit Location form | Edit Location form opens with existing data. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_017 | Update Location with valid data | Location is updated successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_018 | Update only one field | Only the modified field is updated. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_019 | Verify required validation during Edit | Required validation message is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_020 | Cancel Edit Location | Changes are discarded successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_021 | Delete Location successfully | Location is deleted successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_022 | Cancel Delete Location | Location remains unchanged. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_023 | Delete multiple Locations | Selected Locations are deleted successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_024 | Verify Select All checkbox | All rows are selected successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_025 | Verify individual row selection | Selected row is checked successfully. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_026 | Verify sorting by Name | Records are sorted correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_027 | Verify sorting by City | Records are sorted correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_028 | Verify sorting by Country | Records are sorted correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_029 | Verify sorting by Phone | Records are sorted correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_030 | Verify sorting by Number of Employees | Records are sorted correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_031 | Verify Phone field accepts valid characters | Valid phone number is accepted. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_032 | Verify Phone field rejects alphabetic characters | Invalid phone number is rejected. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_033 | Verify Zip / Postal Code accepts numeric value | Numeric Zip / Postal Code is accepted. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_034 | Verify Zip / Postal Code accepts alphanumeric value | Alphanumeric Zip / Postal Code is accepted. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_035 | Verify Zip / Postal Code accepts special characters | Special characters are accepted. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_036 | Verify success toast notification | Success toast notification is displayed. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_037 | Verify total records after CRUD operations | Total record count is updated correctly. | - | ⏳ Not Executed | - | - |
| TC_ADMIN_LOC_038 | Verify existing data is pre-filled during Edit | Existing data is displayed correctly in the Edit form. | - | ⏳ Not Executed | - | - |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 38 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 38 |
| Pass Rate | 0% |

---

# Notes

- Test execution has not been performed yet.
- Actual Result, Status, Evidence, and Bug ID will be updated after each test case is executed.
- Failed test cases will be linked to the corresponding Bug Report.
- Any additional issues discovered during exploratory testing will be documented separately in the Bug Report folder.
