> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

# megane-photo

A web application that automatically overlays Apple Vision Pro-style glasses onto faces in an image using facial landmark detection.

## Demo

**Try it live: [https://code4fukui.github.io/megane-photo/](https://code4fukui.github.io/megane-photo/)**

The application loads with a sample image to demonstrate the effect. You can then drag and drop your own image onto the canvas.

## Features

-   **Simple Interface:** Drag-and-drop an image file to get started.
-   **Automatic Face Detection:** Identifies and processes up to 10 faces in a single image.
-   **Smart Overlay:** Places an image of Apple Vision Pro-style glasses on each detected face.
-   **Dynamic Adjustment:** Automatically calculates the correct size and rotation for the glasses based on the position of the eyes.

## How to Use

1.  **Open the demo link.** A default test image will be displayed with glasses already applied.
2.  **Drag and drop your own image file** onto the web page.
3.  The application will instantly detect the faces and overlay the glasses.

## How It Works

This project uses Google's [MediaPipe Face Mesh](https://chuoling.github.io/mediapipe/solutions/face_mesh.html) library to detect a 3D mesh of facial landmarks directly in the browser.

The application identifies the coordinates for the left and right eyes from the landmark data. It then calculates the distance and angle between these two points to determine the appropriate scale and rotation for the glasses image before overlaying it on the canvas.

## Requirements

-   A modern web browser. No installation is required.

## License

MIT License — see [LICENSE](LICENSE).