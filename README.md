# QRCodeScanner Demo

To get started, create a file `android/local.properties` and indicate your android SDK path. For example:

```
sdk.dir=/Users/nthock/Library/Android/sdk
```

Follow the documentation for installing the React Native QR Code Scanner (https://github.com/moaazsidat/react-native-qrcode-scanner).

Over at the `android/app/build.gradle`, insert this line:

```
android {
  ...
  defaultConfig {
    ...
    missingDimensionStrategy 'react-native-camera', 'general' <-- insert this line
  }
}
```