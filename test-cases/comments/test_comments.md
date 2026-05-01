# Comments Test Cases

---

## TC_006 - Comment Submission

**Preconditions:**
- Post exists
- Comments enabled

**Steps:**
1. Open post
2. Enter name, email, comment
3. Click "Post Comment"

**Expected Result:**
Comment is submitted or marked for moderation

**Priority:** High  
**Status:** Pass  

---

## TC_007 - Comment Management per Role

**Preconditions:**
- Multiple roles exist
- Comments exist

**Steps:**
1. Login as admin/editor
2. Edit/delete/approve comments
3. Login as other roles
4. Verify permissions

**Expected Result:**
Only admin/editor can manage comments

**Priority:** Medium  
**Status:** Pass  

---

## TC_008 - Disable Comments Plugin

**Preconditions:**
- Plugin enabled

**Steps:**
1. Disable comments globally
2. Disable by role
3. Check existing comments

**Expected Result:**
Comments are hidden/disabled correctly

**Priority:** Medium  
**Status:** Pass  
