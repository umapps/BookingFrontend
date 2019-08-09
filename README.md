**Build Android**

In the Project Directory - 
1. `react-native bundle — platform android — dev false — entry-file index.js — bundle-output android/app/src/main/assets /index.android.bundle — assets-dest android/app/src/main/res`
2. `cd android/`
3. `./gradlew assembleDebug`

APK file will be generated in `\android-> app-> build-> outputs-> apk-> debug-> app-debug.apk`. Run `adb install <path-toapk>` to install in Emulator/Physical device


**Build iOS**
1. Open `ios/BookingFrontend.xcworkspace` in Xcode 
2. run `react-native bundle --entry-file index.js --platform ios --dev false --bundle-output ios/main.jsbundle --assets-dest ios` to generate the main.jsbundle
3. Run from Xcode
