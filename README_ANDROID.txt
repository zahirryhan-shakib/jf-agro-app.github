BUILD THE ANDROID APK
This is the Android wrapper project source plus a GitHub Actions workflow that builds a debug APK.
It is not itself an APK file.

EASIEST BUILD ROUTE
1. Create/sign in to a GitHub account.
2. Create a new repository, e.g. jf-agro-app.
3. Upload the CONTENTS of this android-apk-project folder to the repository root (including .github).
4. Open the repository > Actions > "Build Android APK" > Run workflow.
5. When the workflow finishes, open its run page and download the artifact named jf-agro-debug-apk.
6. Extract the downloaded artifact ZIP. It contains app-debug.apk.
7. Transfer app-debug.apk to Android phone and install. Android may ask you to allow installation from that source.

NOTES
- This workflow builds a DEBUG APK for testing. It is not a Play Store release and is not signed with your private release key.
- For public distribution / Play Store, create a release signing key, keep it private, configure GitHub Secrets, and build a signed release APK/AAB.
- You may need to accept Android installation warnings for a debug build.
- The app uses local browser-style storage; it does not yet sync records between phones or to the cloud.
- The APK project wraps the current web app. It does not magically add cloud sync.
