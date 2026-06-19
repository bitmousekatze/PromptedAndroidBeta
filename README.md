# Prompted — Android Beta

Private beta distribution for the **Prompted** Android app.

> **Prompted** — see what tools people are using, the prompts that actually get
> results, and how to apply AI to your own work. Updated daily by the community.

This repo hosts the install page and the latest beta `.apk` for invited testers.

### Latest build — Jun 19, 2026 (build 3)

The soft-launch build. **Push notifications are here** — likes, comments,
replies, @mentions and new direct messages now notify you even when the app is
closed. Plus a round of fixes: the **Communities tab** now loads the full list
in the app (instead of "No communities yet"), **Google/GitHub login** no longer
leaves the login page stuck on screen after you sign in, the **Arena** category
slider no longer yanks the sidebar open when you swipe across it, and **Videos**
now has a back button to exit the view.

Build 2 (Jun 17): blue tap-flash fully gone, bottom system bar hidden, Videos
caption no longer cut off, feed can't scroll behind an open sidebar, login window
closes itself after sign-in, opening notifications marks them all read at once,
chat bubble color & background picker in Messages.

## 📥 Download & install

**→ [Open the install page](https://bitmousekatze.github.io/PromptedAndroidBeta/)**

The page has a one-click download button plus step-by-step instructions for
**BlueStacks (PC)** and **Android phones**.

Prefer the direct file? Grab **[`Prompted-beta.apk`](Prompted-beta.apk)** from this repo.

## 🐞 Found a bug?

Use the **[bug report page](https://bitmousekatze.github.io/PromptedAndroidBeta/bug-report.html)**
— a quick form that sends the report (plus device info) straight to the
maintainer via Formspree. There's also a **Report a bug** button on the install
page.

### Quick steps

**BlueStacks (PC)**
1. Download `Prompted-beta.apk`.
2. Drag the file onto the BlueStacks window (or use the **Install APK** button).
3. Open **Prompted** from the BlueStacks home screen.

**Android phone**
1. Download `Prompted-beta.apk` from the install page.
2. Allow your browser to *install unknown apps* when prompted.
3. Open the file and tap **Install**.

A "Play Protect / unknown sources" warning is expected for a beta build
installed outside the Play Store — tap *Install anyway*.

## ℹ️ Notes

- **Debug/beta build** — expect rough edges; please report bugs.
- **Sign in** with Google, GitHub, or email (same account as the website).
- **Pro** is purchased on the website (`prmpted.com`), not in the app — Play
  Store policy. Pro status carries over once you're signed in.
- Updates are manual during beta: download the newer APK here and install over
  the old one. Your data lives in your account, so nothing is lost.

## 📋 Device compatibility

Works on **any** Android device — real phones, tablets, and emulators like
BlueStacks alike. BlueStacks just runs Android, so anything that installs there
installs on a physical phone too.

| Spec | Value |
|------|-------|
| Package | `com.prmpted.app` |
| Version | 1.0 (versionCode 1) |
| Build type | Debug (debug-signed, for sideloading) |
| File size | ~9.7 MB |
| Minimum Android | **7.0 (Nougat, API 24)** — phones from ~2016 onward |
| Target Android | 16 (API 36) |
| CPU architectures | **All** — no restriction |

Because this is a [Capacitor](https://capacitorjs.com/) WebView app, the APK
contains no native `lib/` binaries, so it's **architecture-independent**: the
same file runs on arm, arm64, x86, and x86_64 without separate builds.

> A "Play Protect / unknown sources" warning is expected for a debug build
> installed outside the Play Store — that's normal for beta testing.

## 🔧 For maintainers

The APK is a debug build of the [Prompted](https://github.com/jackherzlich-ops/Prompted)
Capacitor Android project (`appId com.prmpted.app`):

```bash
# in the prompted repo
npm run android:sync
cd android && ./gradlew assembleDebug
# output: android/app/build/outputs/apk/debug/app-debug.apk
```

Copy that file here as `Prompted-beta.apk`, bump the version note in
`index.html`, then commit and push.

---

*Private beta · not affiliated with Google Play.*
