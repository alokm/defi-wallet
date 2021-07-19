# Mobile App Development Research and Strategy

## Problem with traditional native app development

* Building native apps is expensive and requires completely unique and non-fungible development skills for each of the two major platforms: iOS and Android.
* Building native apps involves acquiring and maintaining two additional technology stacks (Objective-C/Swift and Java/Kotlin) in addition to web
* Building 2 native apps with two separate native technologies adds significant cost, time, and complexity to the project

## Proposed alternative

* Building near-native apps is more cost-effective, faster to market, and easier to recruit talent to contribute to from both the market and the community
* Historically cross-platform mobile dev stacks such as PhoneGap and Cordova worked through a Webview and performance was significantly worse than a native app. 
* Old tech (PhoneGap, Cordova) worked very similar to Electron Apps today in that they were essentially web apps running in a native shell, with degraded webapp performance compared with native.
* New tech (React Native, Expo) are different, better. They use React-like syntax as input that then compiles to native code. The performance is near-native and hardly noticable
* This technology is not for all apps. Works best for apps of low to medium complexity. This is not for a native game or networking app. 
* Some native interfaces exist to low-level hardware such as phone camera and microphone, secure enclave, or gyroscope, etc.
* Where React Native and Expo hit their limits the option exists to 'eject' to native code that interoperates seamlessly
* If the project is successful and little or no native code needs to be generated for either platform (iOS, Android) then it is possible to maintain a nearly uniform single codebase that compiles across platform with only configuration changes
