# Authentication Test Cases

---

## TC_001 - Valid Login & Logout

**Preconditions:**
- Test user accounts exist (Admin, Author, Subscriber)
- User is on login page

**Steps:**
1. Navigate to login page
2. Enter valid credentials
3. Click Login
4. Verify dashboard loads
5. Click Logout
6. Verify redirect to login/home page

**Expected Result:**
User logs in successfully and can log out properly

**Priority:** High  
**Status:** Pass  

---

## TC_002 - Invalid Login

**Preconditions:**
- Login page accessible

**Steps:**
1. Enter invalid username/password
2. Click Login

**Expected Result:**
Error message is displayed and login is denied

**Priority:** High  
**Status:** Pass  

---

## TC_003 - Forgot Password

**Preconditions:**
- User accounts exist

**Steps:**
1. Click "Lost your password?"
2. Enter valid username/email
3. Enter invalid username/email

**Expected Result:**
- Valid → reset process triggered (or error λόγω localhost)
- Invalid → error message shown

**Priority:** High  
**Status:** Pass  
