60 GK Sprint — phone-only APK build guide

This package includes a GitHub Actions workflow to attempt a cloud build of a DEBUG APK. It does not contain a compiled APK yet. The cloud build must run successfully before an APK can be downloaded.

PHONE-ONLY STEPS
1. Download and extract this ZIP on your phone (use your Files app or an archive app).
2. Open github.com in Chrome and sign in or create a GitHub account. Follow GitHub's age and account rules; if needed, ask a parent/guardian to help.
3. Create a new repository named 60-gk-sprint. Keep it private while developing.
4. Upload the files and folders inside the 60_GK_Sprint_Android folder to the repository root. IMPORTANT: include the hidden .github/workflows/android-apk.yml file. If the mobile upload screen hides dot-folders or makes this difficult, use GitHub's web editor to create the workflow file at .github/workflows/android-apk.yml and paste in the workflow from this ZIP.
5. Open the repository's Actions tab. If GitHub asks to enable Actions, enable them for this repository.
6. Select “Build 60 GK Sprint APK” in the workflow list. Press “Run workflow” if shown, or push/commit a file to the main branch to trigger it.
7. Wait for the run to finish. A green check means the build succeeded; a red X means it failed and the log needs checking.
8. Open the successful workflow run, scroll to Artifacts, and download “60-GK-Sprint-debug-apk”. Extract the downloaded artifact ZIP; it contains app-debug.apk.
9. Tap the APK to install. Android may ask you to allow installation from that browser/files app. Only allow it for the APK you built from your own repository, then turn the permission off afterward if desired.

IMPORTANT LIMITATIONS
- This is a DEBUG APK for testing, not a signed release for Google Play.
- The workflow is a starter setup and may need adjustment if GitHub's runner or Capacitor/Android build requirements change.
- Do not upload passwords, signing keys, private tokens, or personal information to the repository.
- Keep the repository private at first.
- The sample PYQ entries in the app are practice questions, not verified verbatim official UPSC/SSC past-year questions.
