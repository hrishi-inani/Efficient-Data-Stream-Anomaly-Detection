# Efficient Data Stream Anomaly Detection

This project implements a robust anomaly detection system for streaming data using the **Robust Random Cut Forest (RCF)** algorithm. The system can efficiently detect outliers or anomalies in sequential data, making it ideal for real-time monitoring applications.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Algorithm Details](#algorithm-details)
- [Results](#results)

## Project Overview
This project simulates a sinusoidal data stream, introduces anomalies, and uses the RCF algorithm to detect them. The project demonstrates RCF’s effectiveness for real-time anomaly detection in evolving datasets.

## Features
- **Synthetic Data Stream Generation**: Creates a time-series data stream with sinusoidal patterns and Gaussian noise.
- **Anomaly Injection**: Adds anomalies to simulate irregularities, such as sudden spikes or drops.
- **Anomaly Detection with RCF**: Uses a forest of Random Cut Trees to identify anomalies based on codisplacement scores.
- **Visualization**: Plots the data stream with anomalies highlighted for easy analysis.

## Installation
1. Clone the repository:
    ```bash
    https://github.com/hrishi-inani/Efficient-Data-Stream-Anomaly-Detection.git
    cd Efficient-Data-Stream-Anomaly-Detection
    ```

2. Install required packages:
    ```bash
    pip install numpy matplotlib rrcf
    ```

## Algorithm Details
The RCF algorithm is ideal for real-time anomaly detection due to its scalability and adaptability:
- **Random Cut Trees (RCT)**: A set of RCTs are used to form a forest, where each tree learns patterns in the data stream and computes codisplacement scores.
- **Codisplacement Score**: Measures the displacement of data points within the trees to identify anomalies based on deviations from typical patterns.
- **Threshold-based Detection**: A score threshold of 1.7 times the previous score is used to flag anomalies.

## Results
The project successfully detects anomalies in a simulated data stream, with anomalies visualized in red for easy identification. The RCF algorithm demonstrates high accuracy and adaptability to data stream changes.
