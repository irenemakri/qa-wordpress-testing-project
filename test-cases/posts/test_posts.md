# Post Management Test Cases

---

## TC_004 - Create & Publish Post

**Preconditions:**
- User logged in (Admin/Editor/Author)

**Steps:**
1. Navigate to Posts → Add New
2. Add title and content
3. Save draft
4. Preview post
5. Publish post

**Expected Result:**
Post is successfully published and visible on frontend

**Priority:** High  
**Status:** Pass  

---

## TC_005 - Image Upload in Post

**Preconditions:**
- Author logged in

**Steps:**
1. Create new post
2. Upload featured image
3. Add image block

**Expected Result:**
Images display correctly without breaking layout

**Priority:** Medium  
**Status:** Pass  

**Notes:**
Image display issue found in one post
