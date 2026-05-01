# Role-Based Access Control (RBAC) Test Cases

---

## MC-RBAC-01 - Admin has full dashboard access

**Preconditions:**
- Valid Administrator account exists

**Steps:**
1. Sign in as Administrator
2. Open Dashboard, Posts, Pages, Media, Comments, Users, Plugins, and Settings
3. Attempt to create a new post
4. Attempt to moderate a comment

**Expected Result:**
Administrator has full access to all sections and actions complete successfully

**Priority:** High  
**Status:** Pass  

---

## MC-RBAC-02 - Editor can manage content but not site settings

**Preconditions:**
- Valid Editor account exists

**Steps:**
1. Sign in as Editor
2. Open Posts, Pages, and Comments
3. Attempt to access Plugins, Settings, and Users
4. Try to edit a post created by another user

**Expected Result:**
Editor can manage content and comments but cannot access admin settings or plugins

**Priority:** High  
**Status:** Pass  

---

## MC-RBAC-03 - Author can create and publish only own posts

**Preconditions:**
- Valid Author account exists
- Another user has existing content

**Steps:**
1. Sign in as Author
2. Create and publish a new post
3. Try to edit another user's post
4. Attempt to access Plugins or Users

**Expected Result:**
Author can manage own posts but cannot edit others' content or access admin settings

**Priority:** High  
**Status:** Pass  

---

## MC-RBAC-04 - Contributor can save drafts but cannot publish

**Preconditions:**
- Valid Contributor account exists

**Steps:**
1. Sign in as Contributor
2. Create a new post
3. Save as draft
4. Attempt to publish the post

**Expected Result:**
Contributor can create drafts but cannot publish posts

**Priority:** High  
**Status:** Pass  

---

## MC-RBAC-05 - Subscriber cannot access content management

**Preconditions:**
- Valid Subscriber account exists

**Steps:**
1. Sign in as Subscriber
2. Try to access Dashboard
3. Try to open Posts, Pages, Media, Comments, Plugins, and Users
4. Try accessing restricted URLs directly

**Expected Result:**
Subscriber can log in but cannot access any content management or admin sections

**Priority:** High  
**Status:** Pass  

---

## MC-RBAC-06 - Restricted direct URLs are blocked for limited roles

**Preconditions:**
- Editor, Author, Contributor, and Subscriber accounts exist

**Steps:**
1. Sign in with a limited role
2. Try to access restricted URLs (e.g. /wp-admin/plugins.php, /wp-admin/users.php)
3. Repeat for each role

**Expected Result:**
Access is denied or redirected; restricted pages are not accessible

**Priority:** High  
**Status:** Pass  

---
