# Bug Reports

---

## BUG-001 - Category page shows no posts

**ID:** A17  
**Severity:** High  
**Priority:** High  

**Test Data:** Admin user  

**Steps to Reproduce:**
1. Go to homepage
2. Click on “Greece” category link

**Actual Result:**
“Nothing Found” message appears and no posts are displayed

**Expected Result:**
Posts under "Greece" category should be displayed

**Notes:**
Same issue observed across multiple users

---

## BUG-002 - Language not applied for German user

**ID:** A5  
**Severity:** High  
**Priority:** High  

**Test Data:** German user  

**Steps:**
1. Login with German user
2. Open homepage
3. Navigate pages

**Actual Result:**
Site remains in English

**Expected Result:**
Site should be displayed in German

**Notes:**
Language inconsistency across users

---

## BUG-003 - Language not applied for Greek user

**ID:** A3  
**Severity:** High  
**Priority:** High  

**Test Data:** Greek user  

**Steps:**
1. Login with Greek user
2. Navigate pages

**Actual Result:**
Site remains in English

**Expected Result:**
Site should be displayed in Greek

---

## BUG-004 - Missing translation fallback

**ID:** A7  
**Severity:** Medium  
**Priority:** Medium  

**Steps:**
1. Open translated page
2. Switch to missing language
3. Open untranslated content

**Actual Result:**
Content not translated

**Expected Result:**
Fallback language or proper handling

---

## BUG-005 - Comments section missing

**ID:** A6  
**Severity:** High  
**Priority:** High  

**Test Data:** Editor  

**Steps:**
1. Open post
2. Try to add comment

**Actual Result:**
Comment section not visible

**Expected Result:**
Comment section should be available

---

## BUG-006 - Comment UI not user-friendly

**ID:** A6  
**Severity:** Low  
**Priority:** Medium  

**Test Data:** Admin  

**Steps:**
1. Open comment section
2. Observe UI

**Actual Result:**
Poor UI / unclear links

**Expected Result:**
Clear and user-friendly interface
