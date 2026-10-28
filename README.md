# 🫰 Snap Vanish

**Snap Vanish** is an experimental Chrome extension that aims to create a Thanos-style dust-dissolve effect during browser-based video calls.

Created by **Sarvesha P** as a first project and a fun experiment with browser-based AI.

## What's in this repository?

The repository currently contains the packaged project archive:

- [snap project final project.zip](./snap%20project%20final%20project.zip) — the extension source files, icons, and bundled MediaPipe assets.

Download and extract the ZIP to access the extension files. The source folder should contain the file named manifest.json.

## Intended features

- Intended support for Google Meet, Microsoft Teams, Zoom on the web, and Instagram
- Finger-snap detection using bundled MediaPipe Hands
- Optional snap-sound confirmation from the microphone
- Person segmentation using MediaPipe Selfie Segmentation
- Dust dissolve animation with configurable duration and direction
- Microphone mute/unmute integration where supported
- Popup controls such as **Snap now** and **Learn empty room**
- Keyboard shortcut: Alt + Shift + S

> **Privacy note:** The project is designed for local browser processing. Review the code and network activity yourself before relying on any privacy claim. Compatibility and behaviour can vary by browser and meeting website.

## Install locally in Chrome

1. Open the repository's ZIP file and click **Download raw file**, or use GitHub's **Code → Download ZIP** option for the repository.
2. Extract the downloaded archive on your computer.
3. Open chrome://extensions in Google Chrome.
4. Turn on **Developer mode**.
5. Click **Load unpacked**.
6. Select the extracted extension folder containing manifest.json.
7. Test the extension carefully before using it in an important meeting.

This is an unpacked developer build, not a Chrome Web Store release.

## How to use

1. Open the extension popup and wait for its status.
2. For the best empty-room background, move out of the camera view.
3. Click **Learn empty room** if that control is available and allow the camera to capture the empty room.
4. Return to the same seat without moving the camera.
5. Use **Snap now**, the keyboard shortcut, or snap detection to test the effect.
6. Test reappearing and microphone behaviour before using it in an actual meeting.

The exact workflow and feature availability depend on the current build and meeting website.

## Tech stack

- JavaScript
- Chrome Extension Manifest V3
- MediaPipe Hands
- MediaPipe Selfie Segmentation
- HTML5 Canvas
- WebRTC stream interception

## Responsible use

- Test before joining an important call.
- Check the meeting platform's mute and camera indicators.
- Do not use visual effects to mislead people in situations where accurate presence matters.
- Respect other participants and the rules of your meeting platform.

## Author

**Sarvesha P**

---

This is an experimental personal project. The listed features describe the intended design; they are not a guarantee that every feature works on every site or browser version.
