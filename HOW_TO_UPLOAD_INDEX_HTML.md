# 📤 How to Upload `index_github.html` to GitHub

## 🎯 Step-by-Step Instructions

### **Option 1: Upload via GitHub Web Interface (Easiest)** ✅

#### **Step 1: Go to Your Repository**
- Open: `https://github.com/TatianaClark/PBI_Student_Checklist`

#### **Step 2: Click "Add file"**
- Look in the top right area where files are listed
- Click the green **"Add file"** button (dropdown menu)
- Select **"Upload files"**

#### **Step 3: Upload the File**
- A file picker will open
- Navigate to: `C:\Users\Tatia\copilotdemo\Checklist_Project\`
- Select **`index_github.html`**
- Click "Open" or drag and drop the file

#### **Step 4: Rename During Upload (IMPORTANT!)**
- After uploading, the filename will show as `index_github.html`
- **Change it to `index.html`** before committing
- Click in the filename field and edit the name

#### **Step 5: Commit the Change**
- Scroll down to "Commit changes" section
- Add message: `Add index.html landing page`
- Click green **"Commit changes"** button

#### **Step 6: Done!** ✅
- Wait 1-2 minutes for GitHub Pages to rebuild
- Visit: `https://tatianaclark.github.io/PBI_Student_Checklist/`
- You should see your landing page!

---

### **Option 2: Git Command Line (For Advanced Users)**

```bash
# Navigate to your local repo folder
cd C:\Users\Tatia\copilotdemo\Checklist_Project\

# Copy the file with the correct name
# (This step depends on your OS - see below)

# Stage the file
git add index.html

# Commit the change
git commit -m "Add index.html landing page"

# Push to GitHub
git push origin main
```

**To rename the file before pushing:**

**Windows PowerShell:**
```powershell
Copy-Item -Path "index_github.html" -Destination "index.html"
```

**Windows Command Prompt:**
```cmd
copy index_github.html index.html
```

---

## 📸 Visual Walkthrough

```
STEP 1: Your GitHub Repo
┌─────────────────────────────────────┐
│ TatianaClark/PBI_Student_Checklist   │
├─────────────────────────────────────┤
│ 📁 Code    📁 Issues    📁 Settings │
│                                     │
│ 📄 power_bi_checklist.html          │
│ 📄 README.md                        │
│ 🖼️  PowerBI_Superhero.png           │
│                                     │
│ [Add file ▼] ← CLICK HERE           │
└─────────────────────────────────────┘

STEP 2: Click Dropdown
┌──────────────────┐
│ Create new file  │
│ Upload files ← CLICK THIS
│ (more options)   │
└──────────────────┘

STEP 3: Select Your File
File Picker Opens
→ Browse to: C:\Users\Tatia\copilotdemo\Checklist_Project\
→ Select: index_github.html
→ Click Open

STEP 4: Rename the File
Before Committing:
Change: index_github.html → index.html

STEP 5: Commit
Message: "Add index.html landing page"
[Commit changes ▼]

STEP 6: Done!
✅ File uploaded as index.html
✅ GitHub rebuilds (1-2 minutes)
✅ Your site now shows landing page!
```

---

## ⚠️ IMPORTANT: Rename to `index.html` !!!

**DO NOT:**
- ❌ Upload as `index_github.html`
- ❌ Upload as `index_github`

**DO:**
- ✅ Upload as `index.html` (final name)

This is critical! GitHub Pages specifically looks for `index.html` as the default homepage.

---

## 📋 Your Final GitHub Structure (After Upload)

```
PBI_Student_Checklist/
├── index.html ✅ ← NEW! (Your landing page)
├── power_bi_checklist.html ✅ (Your checklist)
├── PowerBI_Superhero.png ✅ (Your logo)
└── README.md ✅ (Documentation)
```

---

## 🔍 Quick Checklist

- [ ] Open `https://github.com/TatianaClark/PBI_Student_Checklist`
- [ ] Click "Add file" → "Upload files"
- [ ] Select `index_github.html` from your computer
- [ ] **RENAME to `index.html`** (IMPORTANT!)
- [ ] Commit the change
- [ ] Wait 1-2 minutes
- [ ] Visit your site: `https://tatianaclark.github.io/PBI_Student_Checklist/`
- [ ] See your landing page with button to checklist! 🎉

---

## ❓ FAQ

**Q: Can I rename it after uploading?**
- A: Yes! Upload as-is, then rename using the ✏️ edit button method shown in the other guide

**Q: What if I upload the wrong file?**
- A: No problem! Click the 🗑️ delete icon and upload the correct one

**Q: When will changes appear?**
- A: GitHub Pages rebuilds in 1-2 minutes. If you don't see changes, do a hard refresh: `Ctrl+Shift+R` (Windows)

**Q: Do I need to delete `index_github.html` after?**
- A: Only if you want to keep the repo clean. It won't affect anything if left there

---

**Created**: April 20, 2026  
**For**: Uploading index.html to GitHub  
**Status**: Ready to Use ✅
