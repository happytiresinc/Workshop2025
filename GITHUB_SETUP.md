# 📚 GitHub Setup Guide

This guide will walk you through uploading your Automotive Repair Labour Hour Checker app to GitHub step by step.

## 🚀 Step-by-Step GitHub Upload Process

### Step 1: Create a GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up" if you don't have an account
3. Follow the registration process

### Step 2: Create a New Repository
1. **Log in to GitHub**
2. **Click the "+" icon** in the top right corner
3. **Select "New repository"**
4. **Fill in repository details:**
   - Repository name: `automotive-repair-labour-hour-checker`
   - Description: `A comprehensive mobile app for automotive repair shops`
   - Set to **Public** (or Private if you prefer)
   - ✅ Check "Add a README file" (we'll replace it)
   - ✅ Check "Add .gitignore" and select "Node"
   - Choose a license (MIT recommended)
5. **Click "Create repository"**

### Step 3: Download Your Project Files
Since you're working in a web environment, you'll need to download all your files:

#### Method 1: Individual File Download
1. **Right-click on each file** in your project
2. **Select "Save as"** or "Download"
3. **Maintain the folder structure** as shown below

#### Method 2: Create Archive (if available)
If your development environment supports it, create a ZIP archive of your project.

### Step 4: Prepare Your Local Environment

1. **Install Git** (if not already installed):
   - Windows: Download from [git-scm.com](https://git-scm.com/)
   - Mac: `brew install git` or download from git-scm.com
   - Linux: `sudo apt install git` (Ubuntu/Debian)

2. **Install Node.js** (v18 or higher):
   - Download from [nodejs.org](https://nodejs.org/)

3. **Install Expo CLI**:
   ```bash
   npm install -g @expo/cli
   ```

### Step 5: Upload to GitHub

#### Option A: Using GitHub Web Interface (Easiest)
1. **Go to your new repository** on GitHub
2. **Click "uploading an existing file"** link
3. **Drag and drop all your project files** maintaining folder structure
4. **Write a commit message**: "Initial commit - Automotive Repair App"
5. **Click "Commit changes"**

#### Option B: Using Git Command Line
1. **Clone your repository**:
   ```bash
   git clone https://github.com/yourusername/automotive-repair-labour-hour-checker.git
   cd automotive-repair-labour-hour-checker
   ```

2. **Copy all your project files** into this folder

3. **Add, commit, and push**:
   ```bash
   git add .
   git commit -m "Initial commit - Automotive Repair App"
   git push origin main
   ```

### Step 6: Verify Upload
1. **Go to your GitHub repository**
2. **Check that all files are present**:
   - ✅ app/ folder with all screens
   - ✅ assets/ folder with images
   - ✅ hooks/, types/, utils/, data/ folders
   - ✅ package.json, app.json, tsconfig.json
   - ✅ README.md and other config files

## 📱 Testing Your App

### On Mobile Device (Recommended)
1. **Install Expo Go** on your phone:
   - iOS: [App Store](https://apps.apple.com/app/expo-go/id982107779)
   - Android: [Google Play](https://play.google.com/store/apps/details?id=host.exp.exponent)

2. **Clone and run locally**:
   ```bash
   git clone https://github.com/yourusername/automotive-repair-labour-hour-checker.git
   cd automotive-repair-labour-hour-checker
   npm install
   npx expo start
   ```

3. **Scan QR code** with Expo Go app

### On Web Browser
```bash
npx expo start --web
```

## 🔧 Project Structure
```
automotive-repair-labour-hour-checker/
├── app/
│   ├── (tabs)/
│   │   ├── _layout.tsx
│   │   ├── index.tsx              # VIN Decoder
│   │   ├── labor-guide.tsx        # Labor Hours
│   │   ├── calculator.tsx         # Calculator
│   │   ├── work-order.tsx         # Work Orders
│   │   ├── tire-calculator.tsx    # Tire Calculator
│   │   └── unit-converter.tsx     # Unit Converter
│   └── _layout.tsx
├── assets/
│   └── images/
├── hooks/
│   └── vehicle-store.ts
├── types/
│   └── vehicle.ts
├── utils/
│   ├── vin-decoder.ts
│   ├── labor-calculator.ts
│   └── responsive.ts
├── data/
│   └── labor-hours.ts
├── package.json
├── app.json
├── tsconfig.json
└── README.md
```

## 🎯 Next Steps After Upload

1. **Update repository URL** in package.json (if you can edit it)
2. **Add collaborators** if working with a team
3. **Set up GitHub Pages** for web demo (optional)
4. **Configure GitHub Actions** for CI/CD (advanced)
5. **Add issues and project boards** for task management

## 🆘 Troubleshooting

### Common Issues:
- **Large files**: GitHub has a 100MB file limit
- **Node modules**: Make sure .gitignore excludes node_modules/
- **Permissions**: Ensure repository is public or you have access
- **Git not found**: Install Git first

### Getting Help:
- GitHub Documentation: [docs.github.com](https://docs.github.com)
- Expo Documentation: [docs.expo.dev](https://docs.expo.dev)
- React Native Documentation: [reactnative.dev](https://reactnative.dev)

## 📞 Support
If you encounter issues, check the main README.md for additional support information.
