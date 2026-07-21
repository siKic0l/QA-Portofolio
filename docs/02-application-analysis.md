# Application Analysis

## Application Information

| Item | Description |
|------|-------------|
| Application | OrangeHRM Open Source Demo |
| Application Type | Human Resource Management System (HRMS) |
| Platform | Web Application |
| Primary User Role | Administrator |

---

# Application Overview

OrangeHRM is a Human Resource Management System (HRMS) designed to help organizations manage employee information and internal HR processes through a centralized web-based platform.

The application provides various modules for employee management, attendance, leave management, recruitment, performance evaluation, claims, and internal communication.

---

# User Role

This portfolio uses the **Administrator** account provided by the OrangeHRM Demo.

The Administrator has access to most system modules and management features, making it suitable for end-to-end functional testing.

---

# Module Analysis

## Authentication

### Purpose

Authenticate users before accessing the system.

### Available Features

- Login
- Forgot Password
- Logout
- Change Password

---

## Dashboard

### Purpose

Provide an overview of important HR information and system activities.

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
- Language Package
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

Manage attendance, working hours, and project timesheets.

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

# Initial Business Flow

```text
User Login
      ↓
Dashboard
      ↓
Access Module
      ↓
Perform Business Process
      ↓
Save Changes
      ↓
View Updated Information
      ↓
Logout
```

---

# Modules Selected for Testing

The initial testing scope for this portfolio will focus on the following modules:

- Authentication
- Dashboard
- PIM (Employee Management)

These modules were selected because they represent the application's core business functionality and provide sufficient coverage for demonstrating manual testing techniques.

Additional modules will be included as the portfolio progresses.

---

# Initial Observations

During the initial exploration, several observations were identified:

- Most management modules implement standard CRUD functionality.
- Search functionality is available across multiple modules.
- Administrator has access to nearly all application features.
- Configuration settings are grouped under dedicated administration modules.
- The application follows a consistent navigation structure, making feature discovery straightforward.

---

# Potential Test Areas

The following testing areas have been identified for future testing activities:

- Authentication
- Form Validation
- CRUD Operations
- Search Functionality
- Navigation
- Role-Based Access Control
- Input Validation
- Session Management
- User Interface Consistency
