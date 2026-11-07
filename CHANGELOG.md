## Unreleased

* iOS: a screen covered by another route (a pushed page, a modal bottom
  sheet) no longer catches drags meant for the route on top. Its drag region
  is dropped while it's covered and comes back when it's on top again.

## 0.1.2

* Homepage and README now link to the package's documentation page on flutterdev.in. No code changes.

## 0.1.1

* Documentation only: added a demo GIF showing the keyboard tracking a finger on an iOS simulator. No code changes.

## 0.1.0

* First release.
* `InteractiveKeyboardDismiss`: the keyboard follows the finger when a scroll
  view is dragged into it, then dismisses or springs back.
* iOS: UIKit's own interactive dismissal, driven from Flutter touches
  (verified on iOS 18.6 and 26.0 simulators).
* Android API 30+: `WindowInsetsAnimationControllerCompat` with live
  `viewInsets`; Android 24–29 falls back to dismiss-on-drag.
* `InteractiveKeyboardDismissController`, `InteractiveKeyboardInset`,
  `InteractiveKeyboardInsetBuilder`, `InteractiveKeyboardPadding`,
  `KeyboardDismissThresholds`, `decideKeyboardRelease`,
  `InteractiveKeyboardChannel.diagnostics()`.
* Swift Package Manager and CocoaPods support.
