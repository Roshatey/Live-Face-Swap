# LiveFaceSwap

LiveFaceSwap is a Python-based application that allows real-time face swapping between a live camera feed and any given image. It uses **Dlib** for facial landmark detection and **OpenCV** for image processing and warping.

---

## Features

- Detects facial landmarks using a pre-trained Dlib model.
- Swaps faces between a live webcam feed and an input image.
- Real-time processing with color correction for seamless blending.
- Can handle single face input, with error handling for multiple or no faces detected.

---

## Installation
Clone this repository:
   ```bash
   git clone https://github.com/Rushatey/Live-Face-Swap.git
   cd Live-Face-Swap
   ```
Create a virtual environment and activate it:
```bash
python -m venv venv
source venv/bin/activate       # Linux/Mac
venv\Scripts\activate          # Windows
```
Install required dependencies:
```bash
pip install -r requirements.txt
```
Prepare your images in the images/ folder.

## Usage
1. Swap faces between two images
```bash
python faceSwapper.py
```
The result will be saved as SwappedImage3.jpg.

2. Detect landmarks on an image
```bash
python faceLandmarks.py
```
Displays the image with facial landmarks marked with numbers.

3. Live face swapping using webcam
```bash
python liveFaceSwapper.py
```
Swap your face in real-time with a given image.
Press q to exit.

## Dependencies

  - Python 3.7+
  - OpenCV
  - Dlib
  - NumPy

## Notes
  - Ensure only one face is in the frame for accurate swapping.
  - Lighting conditions may affect blending results.
  - Webcam resolution and frame size may impact performance.
   git clone https://github.com/yourusername/LiveFaceSwap.git
   cd LiveFaceSwap
