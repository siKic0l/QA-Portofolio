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

---

# User Role

This portfolio uses the **Administrator** account provided by the OrangeHRM Demo environment.

The Administrator account provides access to nearly all system modules and administrative features, making it suitable for comprehensive end-to-end functional testing across multiple business workflows.

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

## PIM (Personnel Information Management)

### Purpose

Manage employee records.

### Available Features

- Employee List
- Search Employee
- Add Employee
- Edit Employee
- Delete Employee
- Reports
- Configuration

---

## Leave

### Purpose

Manage employee leave requests and leave records.

### Available Features

- Apply Leave
- My Leave
- Leave List
- Entitlements
- Reports
- Leave Configuration

---

## Time

### Purpose

Manage employee attendance, working hours, and project timesheets.

### Available Features

- Timesheets
- Attendance
- Employee Reports
- Project Reports
- Customer Management

---

## Recruitment

### Purpose

Manage recruitment activities and candidate information.

### Available Features

- Candidates
- Vacancies
- Add Candidate
- Edit Candidate
- Delete Candidate

---

## My Info

### Purpose

Allow users to manage their personal information.

### Available Features

- Personal Details
- Contact Details
- Emergency Contacts
- Dependents
- Immigration
- Job Information
- Salary
- Qualifications

---

## Performance

### Purpose

Manage employee performance evaluation.

### Available Features

- KPI Management
- Performance Reviews
- Performance Tracker

---

## Directory

### Purpose

Search and view employee directory information.

### Available Features

- Employee Search
- Employee Directory

---

## Maintenance

### Purpose

Perform administrative maintenance operations.

### Available Features

- Employee Data Management
- Candidate Data Management
- Record Search

---

## Claim

### Purpose

Manage employee reimbursement and expense claims.

### Available Features

- Create Claim
- Manage Claims
- Expense Types
- Event Configuration

---

## Buzz

### Purpose

Provide an internal social collaboration platform.

### Available Features

- Create Post
- Upload Photo
- Upload Video
- Like
- Comment
- Share
- Events

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
- The application follows a consistent navigation structure, making feature discovery straightforward.
- Similar page layouts and interaction patterns are reused across different modules, improving usability and reducing the learning curve.

---

# Potential Testing Areas

Based on the application exploration, the following areas have been identified for future testing activities.

- Authentication
- Form Validation
- CRUD Operations
- Search Functionality
- Navigation
- Role-Based Access Control
- Input Validation
- Session Management
- User Interface Consistency

---

# Testing Scope

The following modules are planned as part of this manual testing portfolio.

| Module | Status |
|---------|:------:|
| Login | ✅ Completed |
| Dashboard | ⏳ Planned |
| Admin | ⏳ Planned |
| PIM | ⏳ Planned |
| Leave | ⏳ Planned |
| Time | ⏳ Planned |
| Recruitment | ⏳ Planned |
| Performance | ⏳ Planned |
| Directory | ⏳ Planned |
| Claim | ⏳ Planned |
| Buzz | ⏳ Planned |
