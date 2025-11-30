Here is the **easiest way to remember all DVC + Git commands** using a **simple story flow** 👇
(No images, as per your preference.)

---

# ⭐ **EASY MEMORY TRICK — “CODE → TRACK → STORE → SWITCH → RESTORE → PUSH”**

Think of it like steps in a workflow.
Just remember these 7 words:

### **Code → Tag → Track → Remote → Switch → Restore → Push**

Now see how each word maps to commands 👇

---

# ✅ **1. CODE → Make a version tag in Git**

**git tag**
→ Helps in versioning your code.

---

# ✅ **2. TAG → Identify versions**

Use tags or commit ID.

**git log --oneline**
→ To see all commits quickly.

---

# ✅ **3. TRACK → Tell DVC about your data**

**dvc add .\data\customer.csv**
→ DVC starts tracking your data.

The `.csv` file will now be replaced by `.csv.dvc` metadata file.

---

# ✅ **4. REMOTE → Create storage for DVC**

**dvc remote add -d myremote C:\TEMP\campusx-storage**
→ Set a default remote storage for pushing data.

Check `TEMP` folder location:

```
echo %TEMP%
```

---

# ✅ **5. SWITCH → Move to another version**

If you want to switch your Git version:

**git checkout <hash_code>**

---

# ✅ **6. RESTORE → Get matching data from DVC**

After checking out Git commit:

**dvc checkout**
→ Restores the correct version of data files.

If your data is not available locally:

**dvc fetch**
→ Download data from remote
**dvc checkout**
→ Restore correct file versions

---

# ✅ **7. PUSH → Upload everything**

First push your data:

**dvc push**
→ Uploads data to remote storage

Then push your code:

**git push origin main**

---

# 🎯 **SUPER SHORT MEMORY FORMULA**

### **TAG → ADD → REMOTE → CHECKOUT → DVC CHECKOUT → DVC PUSH → GIT PUSH**

Ordered sequence:

1. **git tag**
2. **dvc add file**
3. **dvc remote add**
4. **git checkout hash**
5. **dvc checkout**
6. **dvc push**
7. **git push**

---

If you want, I can convert this into a **PDF cheat sheet**, **flashcards**, or a **1-page revision sheet**.
