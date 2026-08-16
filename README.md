# Face Recognition Attendance System

## Overview

This project is a Python-based Face Recognition Attendance System that automatically identifies registered individuals and records their attendance.

The system uses OpenCV and the LBPH (Local Binary Patterns Histograms) face recognition algorithm. Face samples are captured, converted to grayscale, trained, and then used for real-time face recognition.

## Key Features

- Real-time face detection
- Face sample collection
- 60 face samples per person
- Grayscale face image processing
- LBPH face recognition
- Automatic attendance marking
- Unknown face detection
- Daily attendance records
- CSV-based attendance storage
- Attendance percentage calculation
- Daily attendance reports
- Recognition confidence threshold

## Technologies Used

- Python
- OpenCV
- NumPy
- Pandas
- Pickle
- CSV File Handling
- Haar Cascade Classifier
- LBPH Face Recognizer

## How the System Works

### 1. Face Data Collection

The system captures 60 face samples for each registered person using a webcam.

The detected face is converted into grayscale and resized to `200 × 200` pixels before being saved.

### 2. Face Training

The collected face images are used to train an LBPH face recognizer.

A label map is created to associate each numeric ID with a person's name.

For example:

```python
capture_faces("Noor")
