# megane-photo

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A web application that overlays glasses on a face detected in an image.

## Demo
Try the demo at [https://code4fukui.github.io/megane-photo/](https://code4fukui.github.io/megane-photo/)

## Features
- Detect faces in an uploaded image
- Overlay a pair of glasses on the detected face
- Adjust the glasses size and orientation based on the face

## Requirements
- No external requirements, the application runs in the browser.

## Usage
1. Upload an image by dragging and dropping it onto the canvas.
2. The application will detect the face(s) in the image and overlay a pair of glasses.
3. The glasses will be sized and oriented based on the detected face.

## Data / API
The application uses the [MediaPipe Face Mesh](https://chuoling.github.io/mediapipe/solutions/face_mesh.html) library to detect facial landmarks and position the glasses.

## License
This project is licensed under the MIT License.