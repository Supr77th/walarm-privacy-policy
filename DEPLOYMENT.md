# Privacy Policy Deployment Instructions

## 🎯 Goal
Host your privacy policy on GitHub Pages and get a public URL for Play Store submission.

---

## 📋 Prerequisites

- GitHub account ([Sign up here](https://github.com/join) if you don't have one)
- Git installed on your computer
- Terminal/Command Line access

---

## 🚀 Step-by-Step Deployment

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **"+"** icon (top right corner)
3. Select **"New repository"**
4. Fill in:
   - **Repository name:** `walarm-privacy-policy`
   - **Description:** "Privacy Policy for W Alarm"
   - **Visibility:** ✅ **Public** (must be public for GitHub Pages)
   - ❌ **DO NOT** check "Add a README file"
5. Click **"Create repository"**

### Step 2: Initialize Git in This Directory

Open Terminal and run:

```bash
cd /Users/supreethprabhakar/wtw/nfc-alarm/privacy-policy
git init
git add .
git commit -m "Initial commit: Add W Alarm privacy policy"
```

### Step 3: Connect to GitHub

Replace `YOUR_USERNAME` with your actual GitHub username:

```bash
git remote add origin https://github.com/YOUR_USERNAME/walarm-privacy-policy.git
git branch -M main
git push -u origin main
```

**Example:** If your username is `johndoe`:
```bash
git remote add origin https://github.com/johndoe/walarm-privacy-policy.git
```

### Step 4: Enable GitHub Pages

1. Go to your repository: `https://github.com/YOUR_USERNAME/walarm-privacy-policy`
2. Click **"Settings"** (top menu bar)
3. Click **"Pages"** (left sidebar, under "Code and automation")
4. Under **"Build and deployment"**:
   - **Source:** Deploy from a branch
   - **Branch:** main
   - **Folder:** / (root)
5. Click **"Save"**

### Step 5: Wait for Deployment

- GitHub will deploy your site (takes 1-2 minutes)
- You'll see a message: "Your site is live at https://YOUR_USERNAME.github.io/walarm-privacy-policy/"

### Step 6: Verify It Works

Open your browser and visit:
```
https://YOUR_USERNAME.github.io/walarm-privacy-policy/
```

You should see your privacy policy page! ✅

---

## 📝 Your Privacy Policy URL

**Save this URL - you'll need it for Play Store submission:**

```
https://YOUR_USERNAME.github.io/walarm-privacy-policy/
```

---

## 🔄 Updating the Privacy Policy

When you need to make changes:

```bash
cd /Users/supreethprabhakar/wtw/nfc-alarm/privacy-policy

# Edit index.html (update the "Last Updated" date)

git add .
git commit -m "Update privacy policy"
git push origin main
```

Changes will be live in 1-2 minutes!

---

## ⚠️ Troubleshooting

### "Permission denied" error when pushing
**Solution:** Set up SSH keys or use Personal Access Token
- [GitHub SSH setup guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

### 404 error when visiting the URL
**Solutions:**
- Wait 2-3 minutes after enabling GitHub Pages
- Verify repository is **Public** (not Private)
- Check file is named `index.html` (not `privacy-policy.html`)
- Ensure GitHub Pages is enabled in Settings → Pages

### "Repository not found" error
**Solution:** Make sure you replaced `YOUR_USERNAME` with your actual GitHub username

---

## ✅ Next Steps

Once your privacy policy is live:

1. ✅ Copy the URL: `https://YOUR_USERNAME.github.io/walarm-privacy-policy/`
2. ✅ Add it to Google Play Console (see Play Store Submission Guide)
3. ✅ Add it to your app's Settings screen (optional but recommended)

---

## 🆘 Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics Tutorial](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
