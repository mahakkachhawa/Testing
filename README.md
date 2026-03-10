# Testing
Testing notes and description

https://www.notion.so/Documents-Used-in-testing-31f0387c9d9b80c082c6d53e52dc1b0f?source=copy_link


# Documents Used in testing

# Authentication Module – Login & Register

---

# 1. BRD (Business Requirement Document)

## Objective

The system should allow users to create an account and securely access the application.

## Business Requirements

- Users should be able to **register** for a new account.
- Users should be able to **login** using registered credentials.
- Only **authenticated users** should access the dashboard.

---

# 2. SRS (Software Requirement Specification)

## Functional Requirements

### FR1 – User Registration

- User must enter:
    - Name
    - Email
    - Password
- Email must be unique.
- Password should be at least **6 characters**.

### FR2 – User Login

- User should login using:
    - Email
    - Password

### FR3 – Authentication Validation

- System should validate credentials.
- Invalid credentials should display an **error message**.

### FR4 – Successful Login

- After successful login, user should be redirected to the **dashboard**.

---

# 3. User Stories

## User Story 1 – Registration

**As a new user**, I want to create an account so that I can access the platform.

## User Story 2 – Login

**As a registered user**, I want to login so that I can use the application features.

---

# 4. Acceptance Criteria

## Registration

- User must provide **name, email, password**
- Email must be **unique**
- Password must contain **minimum 6 characters**
- Registration success message should appear

## Login

- User enters **valid email and password**
- System verifies credentials
- User is redirected to **dashboard**
- Invalid credentials should show **error message**

---

# 5. Test Plan

## Module

Authentication (Login & Register)

## Testing Scope

- User registration
- User login validation
- Error message validation

## Testing Types

- Functional testing
- Validation testing
- UI testing

---

# 6. Test Scenarios

## Registration Scenarios

- TS01 – Verify user registration with valid details
- TS02 – Verify registration with existing email
- TS03 – Verify password validation
- TS04 – Verify registration with empty fields

## Login Scenarios

- TS05 – Verify login with valid credentials
- TS06 – Verify login with invalid password
- TS07 – Verify login with unregistered email
- TS08 – Verify login with empty fields

---

# 7. Test Cases

## Registration Test Cases

### TC_REG_01 – Valid Registration

**Steps**

1. Enter name
2. Enter email
3. Enter password
4. Click register

**Expected Result**

User account should be created successfully.

---

### TC_REG_02 – Registration with Existing Email

**Steps**

1. Enter already registered email
2. Enter password
3. Click register

**Expected Result**

System should display **email already exists** error.

---

### TC_REG_03 – Registration with Weak Password

**Steps**

1. Enter password less than 6 characters

**Expected Result**

System should display **password validation error**.

---

## Login Test Cases

### TC_LOGIN_01 – Valid Login

**Steps**

1. Enter valid email
2. Enter valid password
3. Click login

**Expected Result**

User should be redirected to **dashboard**.

---

### TC_LOGIN_02 – Invalid Password

**Steps**

1. Enter valid email
2. Enter incorrect password

**Expected Result**

System should display **invalid credentials** message.

---

### TC_LOGIN_03 – Unregistered Email

**Steps**

1. Enter unregistered email
2. Enter password

**Expected Result**

System should show **user not found** error.

---

### TC_LOGIN_04 – Empty Fields

**Steps**

1. Click login without entering data

**Expected Result**

System should display **required field validation messages**.

---

# Complete Flow

```
BRD
↓
SRS
↓
User Stories
↓
Acceptance Criteria
↓
Test Plan
↓
Test Scenarios
↓
Test Cases



