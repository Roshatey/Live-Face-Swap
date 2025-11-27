# LiveFaceSwap

LiveFaceSwap is a Python-based application that allows real-time face swapping between a live camera feed and any given image. It uses **Dlib** for facial landmark detection and **OpenCV** for image processing and warping.

---

## Features

- Detects facial landmarks using a pre-trained Dlib model.
- Swaps faces between a live webcam feed and an input image.
- Real-time processing with color correction for seamless blending.
- Can handle single face input, with error handling for multiple or no faces detected.

---
## Some Results of Swapped Faces
Donald Trump and Kim Jong Un

![TSK](https://github.com/user-attachments/assets/ddcc4a08-d73e-4577-9972-3beb91c93707)

![KST](https://github.com/user-attachments/assets/f96c635b-75cb-42e6-97e3-41148d5e5a06)

---
Some Results of Landmarks Identified

Example 1

<img width="342" height="481" alt="Example 1" src="https://github.com/user-attachments/assets/58ef2750-9ce5-40ab-8b8c-5c79e2540b58" />

Example 2

<img width="500" height="669" alt="Example 2" src="https://github.com/user-attachments/assets/e0c36686-c613-47d5-83ad-49e6aaee0a22" />

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
