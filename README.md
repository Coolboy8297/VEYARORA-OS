# AI Tracking

A browser-based computer-vision app with live webcam tracking. It runs in the visitor's browser and does not upload the camera feed through this page.

## Features

- **Face detection and tracking** with optional user-labeled face templates.
- **Hand tracking** for up to two hands, drawing 21 landmarks per hand.
- **Body pose tracking** using a lightweight pose model.
- **Object detection** with COCO-SSD MobileNet.
- **All Tracking** mode to combine the available vision tasks.

## Run it

Open the GitHub Pages site in a modern browser over HTTPS, allow camera access, choose a tracking mode, and press **Start camera** or **Load vision model**. The first run downloads model files from third-party CDNs/model hosts, so an internet connection is required.

## Privacy notes

- Camera access is requested only after the visitor presses Start camera.
- Video processing happens in the browser; this app does not send the camera feed to a server.
- Face templates and labels are stored in that browser's local storage. They do not sync to other devices and can be removed using **Forget all saved faces**.
- Only register face templates for people who have agreed to it. This is a lightweight local face-matching demo, not a secure identity-verification system.
- The app loads JavaScript and model assets from third-party CDN and model-host URLs.

## Deployment

The workflow in `.github/workflows/pages.yml` validates the inline JavaScript and deploys the static site to GitHub Pages when enabled for this repository.

Repository: https://github.com/Coolboy8297/VEYARORA-OS
