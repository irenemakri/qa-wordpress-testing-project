# Security Test Cases

---

## TC_014 - Role-Based Access Control

**Preconditions:**
- Multiple roles exist

**Steps:**
1. Login with different roles
2. Try accessing restricted areas

**Expected Result:**
Access is restricted correctly

**Priority:** High  
**Status:** -  

---

## TC_015 - Restricted Admin Access

**Steps:**
1. Login as subscriber
2. Try accessing /wp-admin

**Expected Result:**
Access denied

**Priority:** High  
**Status:** Pass  
