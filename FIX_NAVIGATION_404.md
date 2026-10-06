# 🔧 Fix 404 Error When Clicking Home Button

## ❌ The Problem

When you click **"Home"** from inside the checklist, it gives a **404 error**.

**Current link (broken):**
```html
<a href="index.html">🏠 Home</a>
```

**Why it breaks:**
- GitHub Pages can get confused with relative paths
- Needs to explicitly go back to the root directory

---

## ✅ The Solution

Change the Home link in `power_bi_checklist.html` to one of these:

### **Option 1: Use Relative Path (RECOMMENDED)** ✅
```html
<a href="./">🏠 Home</a>
```

### **Option 2: Use Absolute Path** ✅
```html
<a href="/">🏠 Home</a>
```

### **Option 3: Full Filename** ✅
```html
<a href="index.html">🏠 Home</a>
```
(This might work now since you renamed the file)

---

## 📝 Steps to Fix on GitHub

1. **Go to your repo**: `https://github.com/TatianaClark/PBI_Student_Checklist`

2. **Click on `power_bi_checklist.html`**

3. **Click the ✏️ Edit button** (top right)

4. **Find line 233** (the Home link):
   ```html
   <li><a href="index.html">🏠 Home</a></li>
   ```

5. **Change it to:**
   ```html
   <li><a href="./">🏠 Home</a></li>
   ```

6. **Scroll down and click "Commit changes"**

7. **Wait 1-2 minutes for GitHub Pages to rebuild**

8. **Test it!** Click Home from the checklist - should work now! ✅

---

## 🎯 What You're Changing

```diff
- <li><a href="index.html">🏠 Home</a></li>
+ <li><a href="./">🏠 Home</a></li>
```

**Find Location**: Line 233 in `power_bi_checklist.html`

---

## ✨ Why This Works

- `./` = current directory (the root of your GitHub Pages site)
- When you click it from anywhere, it goes back to `index.html` properly
- GitHub Pages handles the `./ ` correctly and routes to the homepage
- Works consistently on all pages!

---

## 🧪 Test After Fix

1. Go to your site: `https://tatianaclark.github.io/PBI_Student_Checklist/`
2. Click **"Start Learning"** button
3. Inside the checklist, click **"🏠 Home"** in the navigation
4. Should go back to landing page without 404 error! ✅

---

**Created**: April 20, 2026  
**Status**: Ready to Fix  
**Difficulty**: ⭐ Easy
