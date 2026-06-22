# Prompted — Android Beta

Private beta distribution for the **Prompted** Android app.

> **Prompted** — see what tools people are using, the prompts that actually get
> results, and how to apply AI to your own work. Updated daily by the community.

This repo hosts the install page and the latest beta `.apk` for invited testers.

### Latest build — Jun 22, 2026 (build 4)

**Zeo livestreaming is here.** Watch live streams right inside the app, chat live,
and like streams as they happen — and get a notification the moment someone you
follow goes live. Also new: **Community Projects** (share your own build projects
and grade each other's work), plus stability and performance polish across the app.

Build 3 (Jun 19): push notifications for likes, comments, replies, @mentions and
direct messages; Communities tab loads the full list in-app; Google/GitHub login
no longer leaves the login page stuck after sign-in; Arena category slider no
longer yanks the sidebar open; Videos got a back button.

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
| File size | ~7.2 MB |
| Minimum Android | **7.0 (Nougat, API 24)** — phones from ~2016 onward |
| Target Android | 16 (API 36) |
| CPU architectures | **All** — no restriction |

Because this is a [Capacitor](https://capacitorjs.com/) WebView app, the APK
contains no native `lib/` binaries, so it's **architecture-independent**: the
same file runs on arm, arm64, x86, and x86_64 without separate builds.

> A "Play Protect / unknown sources" warning is expected for a debug build
> installed outside the Play Store — that's normal for beta testing.

---

*Private beta · not affiliated with Google Play.*
