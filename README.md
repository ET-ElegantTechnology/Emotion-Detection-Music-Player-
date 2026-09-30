# Emotion-Detection-Music-Player-
# Emotion-Based Music Player

A computer-vision project that uses a webcam to detect facial expressions
and classify the user's apparent emotional state.

The project combines real-time face detection, facial-expression analysis,
ONNX-based emotion classification, and temporal smoothing as the foundation
for an emotion-aware music experience.

## Current Status
In Development

The current implementation successfully processes webcam frames,
detects faces, extracts face regions, classifies facial expressions using
a FER+ ONNX model, and smooths predictions over multiple frames.

Music recommendation, YouTube integration, and the final application
interface are planned components of the project.

## Technology Stack

- Python
- OpenCV
- MediaPipe / BlazeFace
- ONNX Runtime
- FER+ emotion model
- NumPy

## Current Architecture

Webcam
→ Face Detection
→ Face Crop
→ Emotion Classification
→ Emotion Smoothing
→ Music Selection (Planned)

## Project Structure

emotion-based-music-player/
│
├── app.py
├── face_detector.py
├── emotion_detector.py
├── emotion_smoother.py
├── music_service.py
├── youtube_service.py
├── config.py
├── requirements.txt
│
└── models/
    ├── blaze_face_short_range.tflite
    └── emotion-ferplus-8.onnx
