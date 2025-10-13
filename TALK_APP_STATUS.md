# Seventh Star Talk App - Configuration Status

## Overview
Complete rebranding of Nextcloud Talk to **Seventh Star Talk** for Seventh Star (Pty) Ltd educational platform.

---

## ✅ Completed Configuration

### 1. **App Identity**
- **App Name**: Seventh Star Talk
- **Bundle ID**: za.co.seventhstar.talk
- **Display Name**: "Seventh Star Talk"
- **Company**: Seventh Star (Pty) Ltd
- **Copyright**: © 2025 Seventh Star (Pty) Ltd

### 2. **Branding (NCAppBranding.m)**
```objc
talkAppName = "Seventh Star Talk"
filesAppName = "Seventh Star"
bundleIdentifier = "za.co.seventhstar.talk"
groupIdentifier = "group.za.co.seventhstar"
appsGroupIdentifier = "group.za.co.seventhstar.apps"
brandColorHex = "#C62828" (Seventh Star Red)
brandTextColorHex = "#FFFFFF"
privacyURL = "https://seventhstar.co.za/privacy"
pushNotificationServer = "https://push-notifications.nextcloud.com"
isBrandedApp = YES
```

### 3. **App Icons**
✅ All app icons replaced with Seventh Star geometric "S" logo
- 1024×1024 (App Store)
- 180×180 (@3x)
- 167×167 (iPad Pro)
- 152×152 (iPad)
- 144×144 (iPad @2x)
- 120×120 (@2x)
- 114×114 (iPhone @2x)
- 100×100 (iPad @2x)
- 87×87 (@3x)
- 80×80 (@2x)
- 76×76 (iPad)
- 72×72 (iPad)
- 60×60 (@3x)
- 58×58 (@2x)
- 57×57 (iPhone)
- 50×50 (iPad)
- 40×40
- 29×29
- 20×20

### 4. **Launch Screen**
✅ Background color: #C62828 (Seventh Star Red)
✅ Logo: Seventh Star geometric "S" logo (white on red)
✅ All sizes: launchscreen.png, @2x, @3x

### 5. **URL Schemes**
- `nextcloudtalk://` - Standard Talk deep linking
- `seventhstartalk://` - Seventh Star custom scheme

### 6. **App Queries (LSApplicationQueriesSchemes)**
- `nextcloud` - For integration with Seventh Star Files app
- `seventhstar` - Custom Seventh Star scheme
- `nextcloudnotes` - Notes integration
- `firefox` - Browser support

### 7. **Push Notifications**
- Server: https://push-notifications.nextcloud.com
- Configured for APNs integration
- Requires: Apple Developer account with APNs certificate/key

### 8. **Dependencies (CocoaPods)**
✅ All dependencies installed successfully:
- AFNetworking 3.2.0
- DateTools 2.0.0
- MaterialComponents 124.2.0
- MobileVLCKit 3.5.1
- Toast 4.0.0
- MDFInternationalization 3.0.0
- MZTimerLabel 0.5.4
- MotionAnimator 4.0.1
- MotionInterchange 3.0.0

### 9. **Documentation**
✅ ATTRIBUTION.md - GPL-3.0 compliance and attribution
✅ README_SEVENTHSTAR.md - Project information

---

## 🏗️ Build Instructions

### Prerequisites
1. Xcode 14.0 or later
2. macOS with Homebrew
3. Ruby 3.1+ (installed via Homebrew)
4. CocoaPods 1.16+

### Setup
```bash
# Navigate to Talk app directory
cd "/Users/matthew/Desktop/NextCloud IOS Base App/Seventh Star Talk"

# Install dependencies (already done)
pod install

# Open workspace (NOT .xcodeproj)
open NextcloudTalk.xcworkspace
```

### Building
1. Open `NextcloudTalk.xcworkspace` in Xcode
2. Select target: "NextcloudTalk"
3. Select destination: iPhone simulator or device
4. Product → Build (⌘B) or Run (⌘R)

---

## 🔗 Integration with Seventh Star Files App

### URL Scheme Communication
The Talk app can be launched from the Files app using:
- `nextcloudtalk://` scheme for Talk functionality
- Files app uses `seventhstar://` scheme

### Shared App Groups
Both apps share data via:
- `group.za.co.seventhstar` - Main shared container
- `group.za.co.seventhstar.apps` - Apps shared container

This enables:
- Shared user accounts
- Shared server settings
- Cross-app file access
- Unified push notifications

---

## 📋 Remaining Tasks

### Before App Store Submission
1. **Apple Developer Account**
   - Enroll in Apple Developer Program ($99/year)
   - Create App ID: `za.co.seventhstar.talk`
   - Configure Push Notifications capability
   - Create APNs certificate or auth key

2. **Code Signing**
   - Create development certificate
   - Create distribution certificate
   - Create provisioning profiles

3. **App Store Connect**
   - Create app listing for "Seventh Star Talk"
   - Add screenshots (all device sizes)
   - Write app description
   - Set privacy policy URL: https://seventhstar.co.za/privacy
   - Add app category (Social Networking / Education)

4. **Testing**
   - Test on physical iOS devices
   - Verify Talk functionality with seventhstar.co.za server
   - Test push notifications
   - Test integration with Seventh Star Files app
   - Beta testing via TestFlight

---

## 🎨 Brand Consistency

### Colors
- **Primary**: #C62828 (Seventh Star Red)
- **Text on Primary**: #FFFFFF (White)
- **Server Theming**: Enabled (can override with server colors)

### Typography
- Standard iOS system fonts
- Navigation bar: White text on red background

### Logo Usage
- App icon: Geometric "S" on red background
- Launch screen: White "S" on red background
- Navigation logo: Adapts to theme color

---

## 📝 License & Attribution

### License
GPL-3.0-or-later (same as Nextcloud Talk)

### Based On
- Nextcloud Talk iOS
- Copyright © 2020-2025 Nextcloud GmbH and contributors
- Original repository: https://github.com/nextcloud/talk-ios

### Modifications
- Complete rebranding to Seventh Star
- Custom bundle identifiers
- Seventh Star color scheme
- Seventh Star logos and assets
- Modified for educational platform use

### Copyright
Seventh Star modifications - Copyright © 2025 Seventh Star (Pty) Ltd

---

## 🔍 Verification Checklist

✅ App name changed to "Seventh Star Talk"
✅ Bundle ID: za.co.seventhstar.talk
✅ All app icons use Seventh Star logo
✅ Launch screen uses Seventh Star branding
✅ Brand color: #C62828
✅ Copyright updated to Seventh Star (Pty) Ltd
✅ Privacy URL: seventhstar.co.za/privacy
✅ URL schemes configured (nextcloudtalk, seventhstartalk)
✅ App groups configured for integration
✅ Push notification server configured
✅ CocoaPods dependencies installed
✅ Attribution documentation created

---

## 📞 Support

For issues or questions about this branded version:
- Website: https://seventhstar.co.za
- Original Nextcloud Talk: https://github.com/nextcloud/talk-ios

---

**Status**: ✅ **READY FOR TESTING**

The Seventh Star Talk app is fully configured and ready for:
1. Local testing on simulator
2. Device testing (requires code signing)
3. Integration testing with Seventh Star Files app
4. Beta testing via TestFlight
5. App Store submission

Last Updated: October 10, 2025
