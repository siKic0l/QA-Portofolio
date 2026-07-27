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
| Execution Status | Completed |

---

# Test Execution Results

| Test Case ID | Test Case | Expected Result | Actual Result | Status | Evidence | Bug ID |
|--------------|-----------|-----------------|---------------|--------|----------|--------|
| TC_ADMIN_LOC_001 | Verify Locations page loads successfully | Locations page loads successfully. | Locations page loaded successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_001.png) | - |
| TC_ADMIN_LOC_002 | Verify Locations table structure | Locations table displays all expected columns. | Locations table displayed correctly. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_002.png) | - |
| TC_ADMIN_LOC_003 | Search using full Location Name | Matching location is displayed. | Matching location displayed successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_003.png) | - |
| TC_ADMIN_LOC_004 | Search using partial keyword | Matching locations are displayed. | Matching locations displayed successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_004.png) | - |
| TC_ADMIN_LOC_005 | Search using City | Locations from the specified City are displayed. | Locations filtered by City successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_005.png) | - |
| TC_ADMIN_LOC_006 | Search using Country | Locations from the specified Country are displayed. | Locations filtered by Country successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_006.png) | - |
| TC_ADMIN_LOC_007 | Search with no matching result | No matching records are displayed. | No matching records displayed successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_007.png) | - |
| TC_ADMIN_LOC_008 | Open Add Location form | Add Location form is displayed. | Add Location form opened successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_008.png) | - |
| TC_ADMIN_LOC_009 | Add Location with valid data | Location is created successfully. | Location created successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_009.png) | - |
| TC_ADMIN_LOC_010 | Add Location using only required fields | Location is created successfully. | Location created successfully using only required fields. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_010.png) | - |
| TC_ADMIN_LOC_011 | Verify required validation for Location Name | Required validation message is displayed. | Required validation displayed correctly. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_011.png) | - |
| TC_ADMIN_LOC_012 | Verify required validation for Country | Required validation message is displayed. | Required validation displayed correctly. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_012.png) | - |
| TC_ADMIN_LOC_013 | Verify duplicate Location Name validation | Duplicate Location Name is rejected. | Duplicate Location Name rejected successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_013.png) | - |
| TC_ADMIN_LOC_014 | Verify Country dropdown selection | Country is selected successfully. | Country selected successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_014.png) | - |
| TC_ADMIN_LOC_015 | Verify Country selection using keyboard | Country is selected using keyboard navigation. | Country selected successfully using keyboard navigation. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_015.png) | - |
| TC_ADMIN_LOC_016 | Open Edit Location form | Edit Location form opens with existing data. | Edit Location form opened with existing data pre-filled. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_016.png) | - |
| TC_ADMIN_LOC_017 | Update Location with valid data | Location is updated successfully. | Location updated successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_017.png) | - |
| TC_ADMIN_LOC_018 | Update only one field | Only the modified field is updated. | Only the modified field updated successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_018.png) | - |
| TC_ADMIN_LOC_019 | Verify required validation during Edit | Required validation message is displayed. | Required validation displayed correctly. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_019.png) | - |
| TC_ADMIN_LOC_020 | Cancel Edit Location | Changes are discarded successfully. | Changes discarded successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_020.png) | - |
| TC_ADMIN_LOC_021 | Delete Location successfully | Location is deleted successfully. | Location deleted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_021.png) | - |
| TC_ADMIN_LOC_022 | Cancel Delete Location | Location remains unchanged. | Deletion cancelled successfully and location remained unchanged. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_022.png) | - |
| TC_ADMIN_LOC_023 | Delete multiple Locations | Selected Locations are deleted successfully. | Multiple Locations deleted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_023.png) | - |
| TC_ADMIN_LOC_024 | Verify Select All checkbox | All rows are selected successfully. | All rows selected successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_024.png) | - |
| TC_ADMIN_LOC_025 | Verify individual row selection | Selected row is checked successfully. | Individual row selected successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_025.png) | - |
| TC_ADMIN_LOC_026 | Verify sorting by Name | Records are sorted correctly. | Records sorted correctly by Name. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_026.png) | - |
| TC_ADMIN_LOC_027 | Verify sorting by City | Records are sorted correctly. | Records sorted correctly by City. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_027.png) | - |
| TC_ADMIN_LOC_028 | Verify sorting by Country | Records are sorted correctly. | Records sorted correctly by Country. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_028.png) | - |
| TC_ADMIN_LOC_029 | Verify sorting by Phone | Records are sorted correctly. | Records sorted correctly by Phone. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_029.png) | - |
| TC_ADMIN_LOC_030 | Verify sorting by Number of Employees | Records are sorted correctly. | Records sorted correctly by Number of Employees. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_030.png) | - |
| TC_ADMIN_LOC_031 | Verify Phone field accepts valid characters | Valid phone number is accepted. | Valid phone number accepted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_031.png) | - |
| TC_ADMIN_LOC_032 | Verify Phone field rejects alphabetic characters | Invalid phone number is rejected. | Alphabetic characters rejected successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_032.png) | - |
| TC_ADMIN_LOC_033 | Verify Zip / Postal Code accepts numeric value | Numeric Zip / Postal Code is accepted. | Numeric Zip / Postal Code accepted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_033.png) | - |
| TC_ADMIN_LOC_034 | Verify Zip / Postal Code accepts alphanumeric value | Alphanumeric Zip / Postal Code is accepted. | Alphanumeric Zip / Postal Code accepted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_034.png) | - |
| TC_ADMIN_LOC_035 | Verify Zip / Postal Code accepts special characters | Special characters are accepted. | Special characters accepted successfully. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_035.png) | - |
| TC_ADMIN_LOC_036 | Verify success toast notification | Success toast notification is displayed. | Success toast notification displayed correctly. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_036.png) | - |
| TC_ADMIN_LOC_037 | Verify total records after CRUD operations | Total record count is updated correctly. | Total record count updated correctly after CRUD operations. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_037.png) | - |
| TC_ADMIN_LOC_038 | Verify existing data is pre-filled during Edit | Existing data is displayed correctly in the Edit form. | Existing data displayed correctly in the Edit form. | PASS | [View Evidence](../evidence/Admin-Organization-Locations/TC_ADMIN_LOC_038.png) | - |

---

# Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 38 |
| Passed | 38 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 0 |
| Pass Rate | 100% |

---

# Notes

- All planned test cases were executed successfully.
- No functional defects were identified during test execution.
- All execution evidence has been captured and stored in the **evidence/Admin-Organization-Locations** directory.
- Additional exploratory testing may be performed in future testing cycles to identify edge-case scenarios not covered by the current test suite.
