# CyberCore Intelligence

Flutter Android starter app for CyberCore Technologies.

## Included
- Black, electric-blue and red chat UI
- OpenAI and Gemini provider selector
- API-key settings stored locally using Android secure storage
- Tamil/English prompt support (the selected AI responds to the prompt language)
- GitHub Actions workflow to build a release APK in the cloud

## Build locally
1. Install Flutter stable and Android Studio/Android SDK.
2. Run `flutter create . --platforms=android`
3. Run `flutter pub get`
4. Run `flutter build apk --release`
5. APK output: `build/app/outputs/flutter-apk/app-release.apk`

## Build without a laptop
1. Create a GitHub repository and upload the contents of this folder.
2. Open the repository's Actions tab.
3. Select **Build Android APK** and press **Run workflow**.
4. When it finishes, open the workflow run and download the `CyberCore-Intelligence-APK` artifact.

## API keys
Open Settings in the app and add your OpenAI and/or Gemini API key. API providers may charge for usage. Keys are stored on the device, but embedding provider keys in a distributed mobile app is not suitable for a public production release. For public launch, route requests through a secure backend and never share API keys.

This is source code, not a compiled APK. The cloud workflow produces the APK.
