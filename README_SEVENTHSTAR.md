# Seventh Star Talk

A branded version of Nextcloud Talk for iOS, customized for Seventh Star (Pty) Ltd.

## About

Seventh Star Talk is a secure video calling, audio calling, and chat application built on Nextcloud Talk. It provides:
- 📱 Video & audio calls
- 💬 Group and one-on-one chat
- 📞 VoIP functionality
- 🔒 End-to-end encryption
- 📤 File sharing in conversations
- 🎙️ Screen sharing

## Branding

This app has been customized with:
- **App Name:** Seventh Star Talk
- **Bundle ID:** za.co.seventhstar.talk
- **Brand Color:** #C62828 (Seventh Star Red)
- **Company:** Seventh Star (Pty) Ltd
- **Website:** https://seventhstar.co.za

## Server Configuration

This app connects to your Seventh Star Nextcloud server with Talk installed:
- Server URL: https://seventhstar.co.za

## Integration

This app integrates with:
- **Seventh Star Files App** (za.co.seventhstar.ios)
- URL Schemes: `nextcloudtalk://` and `seventhstartalk://`

## Building

### Requirements
- Xcode 15+
- iOS 15.0+
- CocoaPods

### Setup
```bash
cd "Seventh Star Talk"
pod install
open NextcloudTalk.xcworkspace
```

### Build
1. Open `NextcloudTalk.xcworkspace` in Xcode
2. Select your development team in Signing & Capabilities
3. Build and run (⌘R)

## License

GPL-3.0-or-later (same as Nextcloud Talk)

See ATTRIBUTION.md for complete attribution details.

## Original Project

Based on Nextcloud Talk iOS
- Repository: https://github.com/nextcloud/talk-ios
- Copyright © 2017-2025 Nextcloud GmbH
- License: GPL-3.0-or-later
