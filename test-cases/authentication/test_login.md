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

---

## MC-AUTH-01 - Admin login succeeds with valid credentials

**Preconditions:**
- Administrator account exists

**Steps:**
1. Open login page
2. Enter valid admin credentials
3. Click Login

**Expected Result:**
User logs in successfully and is redirected to dashboard

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-02 - Author login succeeds with valid credentials

**Preconditions:**
- Author account exists

**Steps:**
1. Open login page
2. Enter valid author credentials
3. Click Login

**Expected Result:**
User logs in successfully with correct permissions

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-03 - Subscriber login succeeds with valid credentials

**Preconditions:**
- Subscriber account exists

**Steps:**
1. Open login page
2. Enter valid credentials
3. Click Login

**Expected Result:**
User logs in and has limited access

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-04 - Logout ends session

**Preconditions:**
- User is logged in

**Steps:**
1. Click Logout
2. Refresh page

**Expected Result:**
User is logged out and cannot access protected pages

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-05 - Protected pages blocked after logout

**Preconditions:**
- User logged out

**Steps:**
1. Click browser back
2. Refresh protected page
3. Try direct URL

**Expected Result:**
User must login again

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-06 - Login fails with wrong password

**Preconditions:**
- Valid username exists

**Steps:**
1. Enter valid username
2. Enter wrong password
3. Click Login

**Expected Result:**
Login denied with error message

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-07 - Login fails with unknown username

**Steps:**
1. Enter invalid username
2. Enter password
3. Click Login

**Expected Result:**
Login denied

**Priority:** High  
**Status:** Pass  

---

## MC-AUTH-08 - Empty fields validation

**Steps:**
1. Leave fields empty
2. Click Login

**Expected Result:**
Validation error shown

**Priority:** Medium  
**Status:** Pass  

---

## MC-AUTH-09 - Session cannot be restored after logout

**Preconditions:**
- User logged in then logged out

**Steps:**
1. Use browser back
2. Refresh page

**Expected Result:**
User remains logged out

**Priority:** Medium  
**Status:** Pass  

---
