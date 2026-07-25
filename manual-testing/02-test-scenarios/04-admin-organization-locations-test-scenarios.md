# Admin Organization Locations Test Scenarios

## Overview

This document defines the manual test scenarios for the **Locations** feature under the **Admin → Organization** module in the OrangeHRM Demo application.

The objective is to identify all major functional flows and validation areas before designing detailed test cases.

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

# Test Scenarios

| Scenario ID | Test Scenario | Priority |
|-------------|---------------|----------|
| TS_LOC_001 | Verify Locations page loads successfully | High |
| TS_LOC_002 | Verify Locations table structure | High |
| TS_LOC_003 | Verify search using full Location Name | High |
| TS_LOC_004 | Verify search using partial keyword | High |
| TS_LOC_005 | Verify search using City or Country | Medium |
| TS_LOC_006 | Verify search with no matching results | Medium |
| TS_LOC_007 | Verify Add Location form opens successfully | High |
| TS_LOC_008 | Verify adding a Location with valid data | High |
| TS_LOC_009 | Verify required field validation | High |
| TS_LOC_010 | Verify duplicate Location Name validation | High |
| TS_LOC_011 | Verify Country dropdown selection | Medium |
| TS_LOC_012 | Verify Phone field validation | Medium |
| TS_LOC_013 | Verify Zip / Postal Code input | Low |
| TS_LOC_014 | Verify Edit Location | High |
| TS_LOC_015 | Verify Cancel Edit | Medium |
| TS_LOC_016 | Verify Delete Location | High |
| TS_LOC_017 | Verify Cancel Delete | Medium |
| TS_LOC_018 | Verify Multiple Delete | High |
| TS_LOC_019 | Verify Select All checkbox | Medium |
| TS_LOC_020 | Verify table sorting | Medium |
| TS_LOC_021 | Verify success toast notifications | Low |
| TS_LOC_022 | Verify total records update after CRUD operations | Low |

---

# Functional Coverage

| Area | Covered |
|------|----------|
| Page Navigation | ✅ |
| Search | ✅ |
| Add Location | ✅ |
| Edit Location | ✅ |
| Delete Location | ✅ |
| Multiple Delete | ✅ |
| Table Interaction | ✅ |
| Required Validation | ✅ |
| Duplicate Validation | ✅ |
| Country Selection | ✅ |
| Phone Validation | ✅ |
| Zip / Postal Code Input | ✅ |
| Toast Notification | ✅ |
| Total Records | ✅ |

---

# Notes

- These scenarios are created based on the current behavior of the OrangeHRM Demo application.
- Detailed test steps and expected results are documented separately in the **Test Cases** document.
- Additional exploratory scenarios may be added if unexpected behavior is discovered during execution.
