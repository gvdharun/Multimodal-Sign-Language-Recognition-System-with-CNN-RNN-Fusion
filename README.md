# Multimodal Sign Language Recognition System with CNN-RNN Fusion

## Overview

This project implements a real-time Indian Sign Language (ISL) recognition system using a hybrid deep learning approach. It combines hand skeleton and facial expression features to enhance recognition accuracy. The system leverages MediaPipe for landmark extraction and integrates a 1D CNN with an RNN for spatial-temporal feature learning.

## Features

*   **Real-time ISL Recognition:** Processes video streams to recognize sign language.
*   **Hybrid Deep Learning:** Uses a 1D CNN-RNN architecture for effective feature extraction.
*   **MediaPipe Integration:** Employs MediaPipe for hand and facial landmark detection.
*   **Dataset Evaluation:** Trained and evaluated on ISL and ISL-CSLTR datasets.

## System Architecture

1. **Data Acquisition:** Video input (live stream or pre-recorded).

2. **Landmark Extraction:** MediaPipe extracts hand and facial landmarks from each frame.

3. **Feature Vector Construction:** Landmark coordinates are structured into feature vectors.

4. **Spatial Feature Learning:** 1D CNN processes feature vectors to learn spatial patterns.

5. **Temporal Modeling:** RNN (LSTM/GRU) models temporal dependencies across gesture sequences.

6. **Prediction:** The model outputs recognized words or sentences in ISL.

## Usage

1.  **Install Dependencies:** (Provide specific instructions and libraries used, e.g., TensorFlow, Keras, MediaPipe)

    ```
    pip install mediapipe tensorflow keras opencv-python
    ```
2.  **Prepare Dataset:** Organize video data in the specified format.
3.  **Run the System:** Execute the main script to perform real-time sign language recognition.


## Project Objectives

*   Design and implement a real-time ISL recognition system.
*   Integrate hand skeleton and facial expression features.
*   Develop a hybrid deep learning model (1D CNN + RNN).
*   Achieve high recognition accuracy and real-time performance.

## Key Results

*   Demonstrated high accuracy in both alphabe-level and word-level recognition tasks.
*   Achieved real-time operation, suitable for practical deployment.
*   Outperformed traditional methods by combining hand and facial cues with deep learning.

## Project Structure

*   `models/`: Stores the trained models.
*   `src/`: Includes source code for data preprocessing, feature extraction, model architecture, and training.
*   `notebooks/`: Jupyter notebooks used for experimentation and analysis.
