# detox-reactnative

## Prerequisites
- Follow https://wix.github.io/Detox/docs/introduction/getting-started/
1. Install node.js https://nodejs.org/en/download/
2. Install Detox Command Line Tools

### Install Platform-specific Dependencies, Tools and SDKs
- For Android follow https://wix.github.io/Detox/docs/introduction/android-dev-env
1. Install Java https://www.java.com/en/download/help/path.html
2. Install Android Studio https://developer.android.com/studio
3. Set Environment variables for Android SDK https://developer.android.com/studio/command-line/variables
  - Create variable ANDROID_SDK_ROOT and set value = the path to the SDK’s root directory, e.g C:\Users\[user_name]\AppData\Local\Android\Sdk
  - Add the path to the SDK’s root directory into the global PATH on your computer
4. Install Android (AOSP) Emulator from Android Studio
  - Go to the Android Studio
  - Click [Device Manager]
  - Click [Create Device]
  - Select phone of yource choice
  - Click [Next]
  - Select [System Image] a download it
  - Click [Next]
  - Click [Finish]

### Setting up React Native project
- Install Gradle https://www.simplilearn.com/tutorials/gradle-tutorial/gradle-installation
- Install npm install -g react-native-cli
- Install React-native: npm i react-native
- Follow https://reactnative.dev/docs/environment-setup
choco install -y nodejs.install openjdk8
npm install -g react-native-cli
when running [npm run android] error [Cannot read properties of undefined (reading 'transformFile') at Bundler.transformFile] occured
https://stackoverflow.com/questions/69647332/cannot-read-properties-of-undefined-reading-transformfile-at-bundler-transfo

open settings.gradle file in Android studio

- Install Appium inspector https://github.com/appium/appium-inspector/releases
- Install Appium GUI server https://github.com/appium/appium-desktop/releases/tag/v1.22.2
- Set up Appium inspector + GUI server https://github.com/appium/appium-desktop/issues/1927
run emulator, after it is loaded: npm run android

# Setting up Detox & Cucumber
- yarn global add detox-cli && yarn global add npx
- yarn add -D detox@18.16.0 && yarn add -D @cucumber/cucumber && yarn add -D @babel/register
- Follow https://wix.github.io/Detox/docs/api/configuration

