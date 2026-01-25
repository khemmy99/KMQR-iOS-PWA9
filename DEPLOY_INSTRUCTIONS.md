# Deploy KMQR iOS PWA - Commands for khemmy99

## ✅ Files Ready
Location: `C:\KMQR-iOS-PWA\`
- index.html (80 KB)
- icon.png (56 KB)  
- qrcode.min.js (20 KB)

---

## 🚀 EASIEST METHOD: GitHub Desktop (Recommended)

### Step 1: Create Repository on GitHub
1. Go to: https://github.com/new
2. Repository name: `kmqr-ios-pwa`
3. Visibility: **Public** ✅
4. **Do NOT check** "Add README"
5. Click **Create repository**

### Step 2: Upload with GitHub Desktop
1. Download: https://desktop.github.com
2. Install and sign in with your account
3. Click **File** → **Add Local Repository**
4. Click **Choose** → Select `C:\KMQR-iOS-PWA`
5. Click "create a repository" link
6. Click **Publish repository** (top toolbar)
7. Uncheck "Keep this code private"
8. Click **Publish**

### Step 3: Enable GitHub Pages
1. Go to: https://github.com/khemmy99/kmqr-ios-pwa
2. Click **Settings** tab
3. Click **Pages** (left sidebar)
4. Under **Source**, select **main** branch
5. Click **Save**
6. Wait 2 minutes for deployment

### ✅ Your App Will Be Live At:
```
https://khemmy99.github.io/kmqr-ios-pwa/index.html
```

---

## 💻 ALTERNATIVE: Command Line Method

### Step 1: Install Git
Download and install: https://git-scm.com/download/win
- Use default settings
- **RESTART PowerShell** after installation

### Step 2: Create GitHub Repository
1. Go to: https://github.com/new
2. Name: `kmqr-ios-pwa`
3. Visibility: **Public**
4. Click **Create repository**

### Step 3: Run These Commands

```powershell
# Navigate to folder
cd C:\KMQR-iOS-PWA

# Initialize git
git init

# Add all files
git add .

# Set your name and email (first time only)
git config --global user.name "khemmy99"
git config --global user.email "your.email@example.com"

# Commit files
git commit -m "Deploy KMQR iOS PWA v1.0.8"

# Set branch name to main
git branch -M main

# Add your GitHub repository
git remote add origin https://github.com/khemmy99/kmqr-ios-pwa.git

# Push to GitHub (you'll be asked for GitHub username/password)
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to: https://github.com/khemmy99/kmqr-ios-pwa
2. Click **Settings** → **Pages**
3. Source: **main** branch → **Save**
4. Wait 2 minutes

---

## 📱 Install on iPhone

1. Open Safari (must be Safari, not Chrome)
2. Go to: **https://khemmy99.github.io/kmqr-ios-pwa/index.html**
3. Tap **Share** button (box with arrow)
4. Scroll down → **Add to Home Screen**
5. Tap **Add**
6. KMQR icon appears on your home screen! ✅

**First time**: Needs internet to load  
**After that**: Works 100% offline!

---

## 🔄 Update Your App Later

### Via GitHub Desktop:
1. Edit files in `C:\KMQR-iOS-PWA\`
2. GitHub Desktop shows changes
3. Write commit message
4. Click **Commit to main**
5. Click **Push origin**
6. Changes live in 1-2 minutes

### Via Command Line:
```powershell
cd C:\KMQR-iOS-PWA

# Copy updated version
Copy-Item "C:\Users\KM\kmqr_app\kmqr.html" "index.html" -Force

# Commit and push
git add .
git commit -m "Update to v1.0.9"
git push
```

---

## ✅ Verification

After enabling GitHub Pages, check:
- **Repository**: https://github.com/khemmy99/kmqr-ios-pwa
- **Live App**: https://khemmy99.github.io/kmqr-ios-pwa/index.html
- **Deployment Status**: https://github.com/khemmy99/kmqr-ios-pwa/actions

Look for green checkmark ✅ in Actions tab = deployment successful!

---

## 🆘 Troubleshooting

### "git: command not found"
- Download: https://git-scm.com/download/win
- Install, then **restart PowerShell**
- Try again

### "404 Not Found" on GitHub Pages URL
- Wait 3-5 minutes after enabling Pages
- Check repository is **Public** (not Private)
- Go to Settings → Pages → Should see "Your site is live at..."

### Changes not showing on phone
- Hard refresh: Safari → Hold reload → "Reload Without Content Blockers"
- Clear cache: Settings → Safari → Clear History
- Wait 2-3 minutes for GitHub Pages to rebuild

---

## 🎯 Quick Summary

**Easiest Path**:
1. Create repo: https://github.com/new (name: `kmqr-ios-pwa`, Public)
2. Use GitHub Desktop to publish `C:\KMQR-iOS-PWA\`
3. Enable Pages in Settings
4. Share URL: `https://khemmy99.github.io/kmqr-ios-pwa/index.html`

**Total Time**: 5-10 minutes  
**Cost**: FREE forever! 🎉

---

Your files are ready at `C:\KMQR-iOS-PWA\` - just follow the steps above!
