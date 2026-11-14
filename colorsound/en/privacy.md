---
title: ColorSound privacy policy
permalink: /colorsound/en/privacy/
lang: en
---

# ColorSound privacy policy

*Last updated: 14 November 2026.* · [Version française](../../privacy/)

ColorSound is an audio spectrum visualizer for Windows. This page says what it stores, what can leave your PC, and how you stay in control.

## In short

- **ColorSound sends nothing out of your PC.** It does not use the Internet: it sends nothing to the publisher or to anyone, and the publisher receives, stores and sells no data about you.
- **The sound is analyzed in memory, in real time**, to animate the bars. It is never recorded, kept or sent.
- **No account, no ads, no analytics, no tracking.**
- **Your settings and the diagnostic logs stay on your PC.**

## The sound

ColorSound captures the sound your PC plays, on the Windows default output or on the device you choose, with the Windows audio API. It does not use the microphone. From that sound, it works out the level of each frequency band several times per second to animate the bars. The sound itself is never written to disk or transmitted.

## What ColorSound stores on your PC

- Your settings: themes and colors, number of bars and LEDs, scale, opacity, acrylic background and backlighting, position of the widget on the screen, chosen audio source, start with Windows.
- Diagnostic logs, useful when reporting a problem: ColorSound version, starts and stops, state of the sound capture (with the name of the audio device) and errors. They contain nothing of what you listen to.

With the Microsoft Store version, these files are in the private folder of the app, which Windows deletes when you uninstall it. The portable version keeps them in `%LOCALAPPDATA%\ColorSound`.

On the first launch after an update from ColorSound 4, ColorSound takes over the settings that version 4 stored on your PC. They do not leave your PC.

If you turn on the start with Windows, Windows handles it: a startup task for the Microsoft Store version, a startup entry in the registry for the portable version.

## What can leave your PC

ColorSound itself sends nothing. Two things are Microsoft's, not ColorSound's:

- **The Microsoft Store**, which installs ColorSound and its updates. The [Microsoft Privacy Statement](https://privacy.microsoft.com/en-us/privacystatement) applies to it.
- **Windows diagnostic data**: Windows and its components, including the Windows App Runtime that ColorSound relies on, can send diagnostic data to Microsoft according to your settings (Windows Settings › Privacy & security › Diagnostics & feedback). ColorSound receives none of it and cannot see it.

If the Windows App Runtime is missing on your PC (portable version), ColorSound offers to open its download page at Microsoft: nothing is downloaded without you.

## What ColorSound does not do

ColorSound shows no ads, does not measure your use, builds no profile, contains no tracker or analytics tool, and neither sells nor shares any data with third parties.

## Permissions

The Microsoft Store version declares the `runFullTrust` capability, which every packaged Windows desktop app needs to run as a regular program. ColorSound uses neither the microphone, nor the camera, nor your location, and does not read your files.

## Your choices

- Choose the sound shown: ColorSound settings › General › Audio source.
- Turn the start with Windows on or off: ColorSound settings › General › Run when Windows starts, or Windows Settings › Apps › Startup.
- See or delete the diagnostic logs: ColorSound settings › About › Diagnostic logs opens their folder.
- Delete everything: uninstalling ColorSound (Windows Settings › Apps › Installed apps) deletes its settings and logs. For the portable version, delete its folder and `%LOCALAPPDATA%\ColorSound`.

The publisher holds no data about you. For what belongs to Microsoft (Microsoft Store, Windows diagnostic data), you exercise your rights with Microsoft.

## Children

ColorSound collects no data, whatever the age of the person using it.

## Changes

When this policy changes, the date at the top of the page changes too, and important changes are announced in the release notes.

## Contact

A question about this policy? Write to [nvong.dev@gmail.com](mailto:nvong.dev@gmail.com).
