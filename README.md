# Vibes SDK - iOS

An iOS SDK for handling push integration with the [Vibes API][1].
[![Platforms](https://img.shields.io/cocoapods/p/VibesPush.svg)](https://cocoapods.org/pods/VibesPush)

[![Swift Package Manager](https://img.shields.io/badge/Swift%20Package%20Manager-compatible-brightgreen.svg)](https://github.com/apple/swift-package-manager)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)
[![CocoaPods compatible](https://img.shields.io/cocoapods/v/VibesPush.svg)](https://cocoapods.org/pods/VibesPush)

SDK for Vibes push messaging.

- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Requirements

- iOS 9.0+, iOS 10.0+, iOS 11.0+
- Xcode 8.0+, Xcode 9.0+

## Installing the Vibes Push iOS SDK
You can install the Vibes Push iOS SDK by using dependency managers, or by manually integrating it.

### Using CocoaPods Dependency Manager

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects that you can use to install the Vibes Push iOS SDK. Install CocoaPods using the following command:

```bash
$ gem install cocoapods
```

Note: CocoaPods 1.1.0+ is required to build Vibes Push iOS SDK.

Integrate VibesPush into your Xcode project using CocoaPods by specifying one of the following in your `Podfile`:

If your application is swift 3.x compatible, use the following:

```ruby
source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/vibes/pod_specs.git'
platform :ios, '8.0'
use_frameworks!

pod 'VibesPush', '2.0.1.sw3'
```

If your application is swift 4.x compatible, use the following:

```ruby
source 'https://github.com/CocoaPods/Specs.git'
source 'https://github.com/vibes/pod_specs.git'
platform :ios, '8.0'
use_frameworks!

pod 'VibesPush', '2.0.1.sw4'
```

Run the following command:

```bash
$ pod install
```

### Manually Integrating Vibes Push

If you prefer not to use Cocoapods dependency manager, you can manually integrate Vibes Push into your project.

#### Add the VibesPush.framework to Embedded Binaries

1. Download the `VibesPush.zip` from https://github.com/vibes/pod_specs/tree/master/VibesPush/. Version 1.0.x.sw3 are for client applications compatible with Swift 3.x (and Objc) and Version 1.0.x.sw4 are for client applications compatible with Swift 4.x (and Objc).
2. Unzip the archive you'll obtain `VibesPush.framework`.
3. Select your application project in the Project Navigator (blue project icon) to navigate to the target configuration window, then select the application target under the "Targets" heading in the sidebar.
4. In the tab bar at the top of that window, open the "General" panel.
5. Click the `+` button under the "Embedded Binaries" section.
6. Add the downloaded `VibesPush.framework`.
7. You might need to update the `Framework Search Path` in the tab `Build settings` and add the folder containing ` VibesPush.framework`.

And that's it!
