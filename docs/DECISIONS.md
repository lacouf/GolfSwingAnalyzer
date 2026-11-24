# Design decisions

## 2026-11-24: Start with a local macOS app

Use Swift and SwiftUI in Xcode, with video processing on the Mac. This matches the user's MacBook Pro M1 workflow and avoids server setup while validating the idea.

## 2026-11-24: Import two independent phone recordings

The user will record the two camera angles independently and import both files. A shared visible light cue can help align them; provide a manual offset control because capture timing and frame rates may differ.

## 2026-11-24: Begin with 2D pose overlays

Estimate and draw body landmarks separately in each camera view. Defer calibrated multi-camera 3D reconstruction until the basic import, sync, and comparison workflow is useful.

## 2026-11-24: Support the user's existing iPhones

Use the iPhone 16e and iPhone SE (3rd generation) as initial recording devices. Both support rear-camera 1080p slow motion up to 240 fps; the app should preserve original video timing and be validated on actual recordings.
