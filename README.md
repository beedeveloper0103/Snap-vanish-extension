# 🫰 Snap Vanish

**Snap Vanish** is an experimental Chrome extension that aims to create a Thanos-style dust-dissolve effect during browser-based video calls.

Created by **Sarvesha P** as a first project and a fun experiment with browser-based AI.

## Features

- Intended support for Google Meet, Microsoft Teams, Zoom on the web, and Instagram
- Finger-snap detection using locally bundled MediaPipe Hands
- Optional snap-sound confirmation from the microphone
- Person segmentation using MediaPipe Selfie Segmentation
- Dust dissolve animation with configurable duration and direction
- Microphone mute/unmute integration where supported
- Popup controls, including **Snap now** and **Learn empty room**
- Keyboard shortcut: `Alt + Shift + S`
- AI models and processing assets bundled locally

> **Privacy note:** The project is designed for local browser processing. Review the code and network activity yourself before relying on any privacy claim. Compatibility and behaviour can vary by browser and meeting website.

## Install locally (Chrome)

1. Download this repository as a ZIP and extract it, or clone the repository.
2. Open `chrome://extensions` in Google Chrome.
3. Turn on **Developer mode**.
4. Click **Load unpacked**.
5. Select the extracted project folder containing `manifest.json`.
6. Open a supported meeting website and test the extension carefully.

This is an unpacked developer build, not a Chrome Web Store release.

## How to use

1. Open the extension popup and wait for its status.
2. For the best empty-room background, move out of the camera view.
3. Click **Learn empty room** and allow the camera to capture the empty room.
4. Return to the same seat without moving the camera.
5. Use **Snap now**, the keyboard shortcut, or snap detection to test the effect.
6. Test reappearing and microphone behaviour before using it in an actual meeting.

The exact workflow and availability of controls depend on the current build and the meeting website.

## Tech stack

- JavaScript
- Chrome Extension Manifest V3
- MediaPipe Hands
- MediaPipe Selfie Segmentation
- HTML5 Canvas
- WebRTC stream interception

## Project structure

| File / folder | Purpose |
| --- | --- |
| `manifest.json` | Chrome extension configuration |
| `content.js` / `inject.js` | Meeting-page integration |
| `engine.js` / `engine.html` | Local processing engine and visual effect |
| `popup.html` / `popup.js` | Extension popup and settings |
| `background.js` | Extension service worker and shortcut handling |
| `vendor/` | Bundled MediaPipe scripts, models, and WASM assets |
| `icons/` | Extension icons |
| `DEBUGGING.md` | Troubleshooting notes |

## Troubleshooting

See [`DEBUGGING.md`](DEBUGGING.md) for guidance on investigating MediaPipe/WebGL warnings and failed local asset loads.

## Responsible use

- Test before joining an important call.
- Check the meeting platform's mute and camera indicators.
- Do not use visual effects to mislead people in situations where accurate presence matters.
- Respect other participants and the rules of your meeting platform.

## Author

**Sarvesha P**

---

This project is an experimental personal project. Features listed above describe the intended design; they are not a guarantee that every feature works on every site or browser version.
