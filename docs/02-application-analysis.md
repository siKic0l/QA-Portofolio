# Application Analysis

## Application Information

| Item | Description |
|------|-------------|
| **Application** | OrangeHRM Open Source Demo |
| **Application Type** | Human Resource Management System (HRMS) |
| **Platform** | Web Application |
| **Primary User Role** | Administrator |

---

# Application Overview

OrangeHRM is a web-based Human Resource Management System (HRMS) designed to help organizations manage employee information and internal HR processes through a centralized platform.

The application provides multiple business modules covering employee management, attendance, leave management, recruitment, performance evaluation, reimbursement claims, and internal communication.

This portfolio focuses on selected modules that best represent common business workflows and manual testing activities.

---

# User Role

This portfolio uses the **Administrator** account provided by the OrangeHRM Demo environment.

The Administrator account provides access to nearly all system modules and administrative features, making it suitable for end-to-end functional testing across multiple business workflows.

---

# Module Analysis

## Authentication

### Purpose

Authenticate users before accessing the system.

### Available Features

- Login
- Forgot Password
- Change Password
- Logout

---

## Dashboard

### Purpose

Provide an overview of key HR information and system activities.

### Available Features

- Dashboard Summary
- Quick Access Widgets
- Employee Statistics
- System Overview

---

## Admin

### Purpose

Manage system configurations and administrative data.

### Available Features

#### User Management

- Search User
- Add User
- Edit User
- Delete User

#### Job

- Job Titles
- Pay Grades
- Employment Status
- Job Categories
- Work Shifts

#### Organization

- General Information
- Locations
- Organization Structure

#### Qualifications

- Skills
- Education
- Licenses
- Languages
- Memberships

#### Nationalities

- Manage Nationalities

#### Corporate Branding

- Logo
- Banner
- Color Palette
- Login Banner
- Social Media Images

#### Configuration

- Email Configuration
- Email Subscription
- Localization
- Language Packages
- Modules
- OAuth Client
- LDAP Configuration

---

# Business Flow Overview

The following diagram illustrates the general workflow performed by an administrator when interacting with the system.

```text
User Login
      │
      ▼
Authentication
      │
      ▼
Dashboard
      │
      ▼
Select Module
      │
      ▼
Perform Business Process
      │
      ▼
Submit Changes
      │
      ▼
System Validation
      │
      ▼
Data Updated
      │
      ▼
Logout
```

---

# Initial Observations

The following observations were identified during the initial exploration of the application.

- Most management modules implement standard CRUD (Create, Read, Update, Delete) operations.
- Search functionality is consistently available across multiple modules.
- The Administrator role has access to nearly all system features.
- Configuration settings are centralized within dedicated administration modules.
- The application follows a consistent navigation structure.
- Similar page layouts and interaction patterns are reused across different modules, improving usability and consistency.

---

# Functional Areas Covered

Based on the selected project scope, the completed modules collectively cover the following functional areas:

- User Authentication
- CRUD Operations
- Search Functionality
- Table Sorting
- Form Validation
- Required Field Validation
- Duplicate Data Validation
- Success Notifications
- Error Handling
- Administrative Configuration
- UI Consistency

---

# Testing Scope

This portfolio intentionally focuses on representative OrangeHRM modules that demonstrate the complete manual testing workflow.

The selected modules provide sufficient complexity to showcase professional Quality Assurance practices without introducing repetitive testing across similar business modules.

| Module | Coverage |
|---------|----------|
| Authentication - Login | User Authentication |
| Admin - User Management | User CRUD Operations |
| Admin - Job Titles | Configuration Management |
| Admin - Organization - Locations | Organization Configuration |

---

# QA Coverage

The completed project demonstrates practical experience in:

- Requirement Analysis
- Application Analysis
- Test Planning
- Test Scenario Design
- Test Case Design
- Manual Test Execution
- Exploratory Testing
- Evidence Collection
- Bug Reporting
- Test Summary Reporting
- Test Management using Qase.io

---

# Scope Justification

Rather than testing every module available in OrangeHRM, this project focuses on a carefully selected scope that represents the most common administrative workflows.

These modules collectively demonstrate:

- Authentication
- Business Configuration
- CRUD Operations
- Search and Filtering
- Validation Rules
- Administrative Features
- Functional Verification

This approach reflects real-world QA practices, where testing is performed based on defined project scope and business priorities rather than exhaustive coverage of every available feature.

---

# Conclusion

The selected OrangeHRM modules provide comprehensive coverage of common web application functionality and demonstrate the complete manual testing process from planning through execution and reporting.

This repository represents a completed Manual Testing portfolio project and serves as a practical demonstration of industry-standard QA documentation, structured testing practices, and real-world test management using Qase.io.
