# Login Test Cases - Sauce Demo

## Feature: Login

---

### TC-001: Valid Login

**Preconditions:**
User is on login page

**Test Data:**
Username: standard_user
Password: secret_sauce

**Steps:**
1. Enter username
2. Enter password
3. Click Login button

**Expected Result:**
User successfully redirected tothe inventory page

---

### TC-002: Invalid Password

**Preconditions:**
User is on Login page

**Test Data:**
Username: standard_user
Password: wrong_password

**Steps:**
1. Enter username
2. Enter incorrrect password
3. Click Login button

**Expected Result:**
Error message is displayed

---

### TC-003: Locked Out User

**Preconditions:**
User is on login page

**Test Data:**
Username: locked_out_user
Password: secret_sauce

**Steps:**
1. Enter credentials
2. Click Login button

**Expected Result:**
User is blocked with locked-out error meassage
