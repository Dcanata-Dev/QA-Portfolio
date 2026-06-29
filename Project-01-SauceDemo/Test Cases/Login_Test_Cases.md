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

### TC0003: Empty User Name

**Preconditions:**
Empty Username

**Test Data:**
Username: blank
Password: secret_sauce

**Steps:**
1. Enter blank username
2. Enter password
3. click Login button

**Expected Result:**
User should remain on login page and see an error indicating account has been locked

---

### TC-004: Empty Password

**Preconditions:**
Empty Password

**Test Data:**
Username: standard_user
Password: blank

**Steps:**
1. Enter username
2. Enter blank password
3. Click Login button

**Expected Result:**
Password required message

### TC-005: Both fields empty

**Precondition:**
Both fields empty

**Test Data:**
Username: emtpy
Password: empty

**Steps:**
1. username blank
2. password blank
3. Click Login button

**Expected Result:**
Username required message

### TC-006: Locked Out User

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
