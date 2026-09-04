# ISBM University – Fee Structure & Management Portal 🏛️

A modern, responsive, and real-time Fee Structure Management Portal for ISBM University Raipur Chhattisgarh.

## 🚀 Features
- 📊 **Dynamic Program & Fee Table:** 40+ programs across multiple schools with duration, eligibility, university fee, extra charges, commission, and total calculations.
- 💾 **Cloud & Backup Management:**
  - Full JSON backup export & restore
  - Clear all data with 1-click restore to defaults
  - Admin password management
- 📁 **CSV Import / Export:**
  - Export fee table to CSV (Excel compatible)
  - Download standard CSV template
  - Upload CSV to update or add programs
  - Manual "Add Program" interface
- 💬 **WhatsApp Quotation Generator:** Share instant quotations with prospective students via WhatsApp with custom messaging.
- ⚡ **Firebase Real-Time Cloud Sync:** Real-time synchronization using Google Firebase Firestore (`console.firebase.google.com`).
- 🌐 **Deploy Ready:** Preconfigured for **Vercel** (`vercel.json`) and **Firebase Hosting** (`firebase.json`).

---

## 🛠️ Step 1: Push to GitHub

### Option A: Via GitHub Website (Easiest - No Git installation needed)
1. Go to [github.com](https://github.com/) and create a new repository (e.g., `isbm-fee-portal`).
2. Click **"uploading an existing file"**.
3. Drag and drop all files from this folder (`index.html`, `vercel.json`, `firebase.json`, `.gitignore`, `README.md`).
4. Click **"Commit changes"**.

### Option B: Via Git CLI (if Git is installed)
```bash
git init
git add .
git commit -m "Initial commit of ISBM Fee Portal"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/isbm-fee-portal.git
git push -u origin main
```

---

## 🌐 Step 2: Deploy to Vercel (Free & Instant)
1. Go to [vercel.com](https://vercel.com/) and sign in with your GitHub account.
2. Click **"Add New..."** ➔ **"Project"**.
3. Select your `isbm-fee-portal` repository.
4. Keep the default settings (Framework Preset: *Other*) and click **"Deploy"**.
5. Within 30 seconds, your site will be live with an address like:  
   `https://isbm-fee-portal.vercel.app`

---

## 🔥 Step 3: Connect Google Firebase Cloud Database (`console.firebase.google.com`)

To enable live real-time cloud data storage across all devices:

1. Open [Firebase Console](https://console.firebase.google.com/) and sign in with your Google account.
2. Click **"Add project"** (e.g. `isbm-fees-portal`).
3. Click **"Build"** in the left menu ➔ **"Firestore Database"** ➔ **"Create database"**.
4. Choose **"Start in test mode"** (allows reads and writes) and click **"Enable"**.
5. In Project Overview, click the Web icon `</>` to register a web app.
6. Copy your `firebaseConfig` object, which looks like this:
   ```javascript
   const firebaseConfig = {
     apiKey: "AIzaSy...",
     authDomain: "isbm-fees.firebaseapp.com",
     projectId: "isbm-fees",
     storageBucket: "isbm-fees.appspot.com",
     messagingSenderId: "123456789",
     appId: "1:123456789:web:abcdef"
   };
   ```
7. In the Fee Portal website:
   - Login as Admin (Default password: `isbm2025`).
   - Click **"🔥 Firebase Cloud"** in the Cloud & Backup panel.
   - Paste your config and click **"Connect Firebase"**.
8. Done! All updates, CSV imports, and fee edits will now save in real-time in Google Firebase Cloud Database!
