# Refurbished Display & MF.Installer

Give any Android app a fresh launcher **icon and name** — without cloning it or
touching its original code — and install, convert and manage packages from one
place, optionally with Shizuku.

> **Add-only by design.** Refurbishing an APK keeps its package name, every
> original DEX and all original logic intact. It only *adds* one small module
> (its own namespace) plus minimal manifest/resource entries. The original app
> and the added module stay two separate things.
---

## 📥 DOWNLOAD (Android)
Here: **[Get Lastest](https://github.com/jowafieuzu/MFInstaller/releases/latest)**

## 🐛 Report & Feedback

If you get issue or give a feedback: **[Issues](https://github.com/jowafieuzu/MFInstaller/issues/new)**.

## What it does

### Change Display — refurbish an APK
Pick an app or a package file, add one or more **name + icon** styles, choose a
signing key, and get a refurbished build you can install or save. On your home
screen the app shows the icon and name you chose when you PRESS&HOLD icon app on launcher; the real app underneath is
unchanged. A built-in **Change Display** shortcut lets you switch between the
styles later.

### Installer
A rootless integrated installer (an SAI-style replacement) for:
- Single **APK**
- Split bundles: **APKS**, **APK+**, **XAPK**, **APKM** (merges to a single APK
  on request)
- **OBB** expansion files (direct write on Android ≤10; SAF folder grant on
  Android 11+, still rootless)

Install from an installed app, a file, the in-app APKMirror/APKPure browser, or
“Open with”. Signatures are compared before installing: same key updates in
place, a different key offers to uninstall first.

**Re-sign & install:** pick a package from storage and install it re-signed with the key chosen in Step 3 (no
refurbishing involved; the picked file is never modified), so a manually downloaded newer version can always
install over the previous one.

### Signing — four modes
- **Default · official public key** — the shared, non-secret default key (fine for
  personal use).
- **Private · device keystore** — generated in secure hardware; cannot be
  exported.
- **Portable P12** — generated here and **backup-/import-able** across devices.
- **Custom · JKS / P12 / PFX** — your own keystore (type detected by content,
  not by extension; JKS read natively).

### Advanced — with Shizuku (no root)
Once Shizuku shell access is granted, installs go through the shell silently,
with options: keep data when replacing (same-signature), allow downgrade,
back up & restore app data, grant all permissions, bypass low target-SDK,
enable rollback, spoof installer source. Plus an optional **default-installer /
silent-update** mode, reliable **self-update**, and an **installed-apps**
manager: uninstall from / reinstall for user 0, freeze/unfreeze, restore
rollback, and install into / uninstall from another user profile (e.g. cloning
an app into the Dual Messenger profile).

A bundled in-app **wiki** (English, Vietnamese, Chinese, Korean, Japanese, Russian, Spanish, Italian, French, Arabic, Hindi) walks through both parts. The app UI is available in the same languages; any other system language falls back to English.

---
