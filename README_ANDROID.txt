60 GK Sprint — Android APK starter package

WHAT THIS IS
- A mobile-first HTML/JavaScript app with History, Geography, Polity and Science quizzes.
- Mixed GK sprint, multiple-choice answers, explanations, score summary.
- PYQ Practice Bank with exam/subject filters and answer explanations.
- The starter PYQ bank is explicitly labelled practice content, NOT verified verbatim official UPSC/SSC past-paper questions.

IMPORTANT
This package is the web app source, not a compiled APK. Building a signed Android APK requires Android build tooling (Android Studio/Gradle) or a cloud build service. This environment did not compile or test an APK.

RECOMMENDED BEGINNER ROUTE: BUILD APK WITH ANDROID STUDIO + CAPACITOR
1. Install Node.js LTS and Android Studio on a computer.
2. Extract this ZIP.
3. In the extracted folder, create package.json with:
   {
     "name": "60-gk-sprint",
     "version": "1.0.0",
     "private": true,
     "scripts": {"build": "echo static web app"}
   }
4. Open a terminal in the extracted folder and run:
   npm install @capacitor/core @capacitor/cli
   npx cap init "60 GK Sprint" "com.sixtygksprint.app" --web-dir=www
   npm install @capacitor/android
   npx cap add android
   npx cap sync android
   npx cap open android
5. Android Studio opens the project. Allow Gradle sync and install the recommended Android SDK if asked.
6. For a phone test, enable Developer options and USB debugging on your Android phone, connect it by USB, then press Run in Android Studio.
7. To create an APK: Build > Build Bundle(s) / APK(s) > Build APK(s). The exact menu can vary by Android Studio version.
8. Before public release, configure app icon, version, privacy policy if collecting data, and signing. Google Play generally expects an Android App Bundle (AAB) for new app submissions; APK is useful for direct testing/sharing.

NO COMPUTER?
- You can edit/test the HTML in a mobile browser, but reliably producing and signing an APK is much harder on phone-only workflows. Use a trusted cloud build service or borrow a computer. Never upload signing keys or passwords to an untrusted service.

PYQ CONTENT
- Add official PYQs only after checking original UPSC/SSC papers and answer keys. For each item store exam, year, paper/shift if applicable, subject, question, options, official answer, explanation, and source/reference. Do not label invented practice questions as past-year questions.
