# YappYapp

YappYapp is a local-only dictation app for your Mac. Press Option+Space, talk, and verified text lands where your cursor is, with on-device Whisper and Parakeet transcription so your voice never leaves your Mac.

This repo hosts the public downloads. You are here as a beta friend, so thank you for kicking the tires.

## Install via DMG

1. Download the latest `YappYapp-x.y.z.dmg` from the [Releases page](https://github.com/matd97/yappyapp-releases/releases/latest).
2. Open the DMG and drag YappYapp into your Applications folder.
3. First open, because the app is not notarized yet:
   - **macOS 15 or newer:** double-click YappYapp. macOS will block it. Go to System Settings -> Privacy & Security, scroll to the note about YappYapp, and click **Open Anyway**. Confirm once more when prompted.
   - **macOS 14:** right-click YappYapp in Applications and choose **Open**, then click **Open** in the dialog.

You only do this once. After that YappYapp launches like any other app.

## Install via Homebrew

If you use the tap, one command installs everything:

```
brew install --cask matd97/tap/yappyapp
```

Note: recent Homebrew versions keep macOS quarantine on downloads, so the first-open steps above apply to Homebrew installs too. If you want to skip the first-open prompt entirely, run this after installing:

```
xattr -dr com.apple.quarantine /Applications/YappYapp.app
```

If you would rather skip the first-open Gatekeeper prompt entirely, use the zero-prompt variant:

```
```


## Updates

The app updates itself. Signed updates are delivered through Sparkle, so you get new versions verified and in place without hunting down a download.

## What to test as a beta friend

- Dictate into a few different apps (notes, chat, your editor, a browser field) and see where the text lands.
- Try the languages you actually work in and check how it handles them.
- Teach it your words in the Words tab: product names, clients, acronyms. Watch it correct them across transcripts.
- Meet your pet. Dictate a bit and see it level up.

If something breaks, please [open an Issue](https://github.com/matd97/yappyapp-releases/issues). The app also has built-in diagnostics for mic, models, paste, and permissions, so mention that output in your report and it will save us both time.

## One honest note

The source code is private during this beta. It opens up with the public launch.
