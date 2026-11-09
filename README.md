# Real-Time Pedestrian Detection and Alert System

## Project Overview

This project implements a pedestrian detection and alert system using Python, OpenCV, and the Histogram of Oriented Gradients (HOG) with a Support Vector Machine (SVM) detector.

The system processes video frames to detect pedestrians, estimate their approximate distance from the camera, and classify their movement as standing or walking.

## Features

- Pedestrian detection using HOG + SVM.
- Image processing using OpenCV.
- Approximate pedestrian distance estimation.
- Basic movement classification.
- Visual bounding boxes and distance labels.
- Pushbullet notifications for nearby pedestrians.

## Technologies Used

- Python
- OpenCV
- NumPy
- Requests
- Jupyter Notebook
- Pushbullet API

## Project Structure

- `pedestrian_detection.ipynb` – Main implementation and executed notebook.

## How It Works

1. Loads a video file.
2. Processes individual video frames.
3. Detects pedestrians using the HOG + SVM model.
4. Estimates distance using an assumed focal length and pedestrian height.
5. Classifies movement based on changes in vertical position.
6. Displays detection results through bounding boxes and labels.
7. Sends notifications when a pedestrian is detected within the configured distance threshold.

## Running the Project

Open the Jupyter Notebook in Google Colab, upload a video file, and execute the notebook cells in order.

## Note

Distance estimation is approximate and depends on camera calibration and assumptions about pedestrian height. Movement classification is a basic implementation.

This project was developed as part of my Final Year Project.
