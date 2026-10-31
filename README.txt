BROTHER JARJU ONLINE CLASS — FREE ANDROID PWA SHELL

WHAT THIS PACKAGE DOES
- Adds an installable Progressive Web App shell around your existing Google Apps Script portal.
- Keeps your existing Apps Script + Google Sheets backend and student/admin login.
- Caches only the public app shell. It deliberately does NOT cache private portal pages, logins,
  student records, quiz answers, Drive files or other authenticated data.
- The portal itself still requires internet access for live data and account actions.

FREE HOSTING OPTION: GITHUB PAGES
1. Sign in to https://github.com (create a free account if needed).
2. Create a new PUBLIC repository named: brother-jarju-online-class-app
3. Upload every file and folder in this package to the repository root. Keep the folder structure:
   index.html
   manifest.webmanifest
   service-worker.js
   icons/icon-192.png
   icons/icon-512.png
4. Open the repository Settings > Pages.
5. Under Build and deployment, choose Deploy from a branch.
6. Select branch main and folder /(root), then Save.
7. Wait for GitHub Pages to publish. Your app address will look like:
   https://YOUR-GITHUB-USERNAME.github.io/brother-jarju-online-class-app/

INSTALL ON ANDROID
1. Open the GitHub Pages app address in Google Chrome on Android.
2. Wait for the page to load, then use Chrome's menu (three dots).
3. Choose Install app or Add to Home screen (wording varies by Android/Chrome version).
4. Confirm. The Brother Jarju icon will appear on the home screen/app list.

IMPORTANT TESTING
- First test the hosted URL on Android Chrome before distributing it to students.
- Sign in and test lectures, audio/video, quizzes, results, forms, and logout.
- If the embedded portal shows a browser/Google sign-in error, tap Open Portal in the header.
- If the portal works in the Open Portal tab but not inside the frame, this is an embedding/browser
  restriction to diagnose; do not change your Apps Script deployment access blindly.
- Apps Script deployment must remain available to the intended students. The PWA wrapper does not
  bypass Apps Script permissions or quotas.
- This is a web app installed from Chrome, not a Play Store APK. No Play Store account is needed.

UPDATES
Replace the uploaded PWA files in the GitHub repository when the wrapper changes. The Apps Script
portal continues to be updated separately through Deploy > Manage deployments > Edit > New version.
