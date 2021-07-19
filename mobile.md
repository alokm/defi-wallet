# Mobile App Development Research and Strategy

## Problem with traditional native app development

* Building native apps is expensive and requires completely unique and non-fungible development skills for each of the two major platforms: iOS and Android to acquire and maintaining in-house expertise on two new additional technology stacks in addition to web i.e. Objective-C/Swift and Java/Kotlin.

* Building 2 native apps with two separate native technologies adds significant cost, time, and complexity to the project

## Proposed alternative

* Building near-native apps is more cost-effective, faster to market, and easier to recruit talent to contribute to from both the market and the community

* Historically cross-platform mobile dev stacks such as PhoneGap and Cordova worked through a Webview and performance was significantly worse than a native app. 

* Old tech (PhoneGap, Cordova) worked very similar to Electron Apps today in that they were essentially web apps running in a native shell, with degraded webapp performance compared with native.

* New tech (React Native, Expo) are different, better. They use React-like syntax as input that then compiles to native code. The performance is near-native and the performance difference is hardly noticable in most cases since all views are rendered using native components leaving the only performance difference being that Javascript or Typescript are used for app orchestration code vs native.

* This technology is not for all apps. 
  * It works best for apps of low to medium complexity and covers most apps that do not offer videogame refresh rates or rich media streaming
  * This is not a good choice for a native video game, streaming  or networking app. 

* Some native interfaces exist to low-level hardware such as phone camera and microphone, secure enclave, or gyroscope, etc.
* Where React Native and Expo hit their limits the option exists to 'eject' to native code that interoperates seamlessly
  * But it is ideal if we can avoid writing any custom platform-specific code for iOS or Android

* If the project is successful and little or no native code needs to be generated for either platform (iOS, Android) then it is possible to maintain a nearly uniform single codebase that compiles across platform with only configuration changes

* If we are successful in building a single codebase that cross-compiles to both Android and iOS we can expect to **save 30-40% of the time and cost vs building two native apps from scratch**. 
  * This savings continues to compound over time as we continue to develop and maintain the app
  * The biggest benefit of a common codebase compiling cross-platform is reduced complexity which makes everything faster and easier


