# @punosmobile/react-native-device-brightness

This is a native module for React Native to control the screen brightness.

It is a fork of https://github.com/adrianso/react-native-device-brightness, and has been updated to work with:
- Android SDK 35
- React Native 0.79.0
- iOS 15

## Installation

```
yarn add @punosmobile/react-native-device-brightness
```

## Linking

This module supports auto-linking for React Native version 0.60 and above. No additional steps are required.

## Usage

**Important: Brightness Level only accept value 0 to 1.**

- _Adjusting screen brightness will make iOS's Auto-Brightness function do nothing._
- _Adjusting screen brightness in Android only works in App and will reset to system setting exiting App._

```javascript
import DeviceBrightness from 'react-native-device-brightness';

// Setting brightness
DeviceBrightness.setBrightnessLevel(brightness);

// Getting brightness
const brightness = await DeviceBrightness.getBrightnessLevel();
console.log(brightness);

// Getting system brightness (Android only)
const brightness = await DeviceBrightness.getSystemBrightnessLevel();
console.log(brightness);
```

## License

This software is licensed under the [MIT License](https://github.com/punosmobile/react-native-device-brightness/blob/master/LICENSE).
