# Teachable Machine ML Model Guide

This guide provides step-by-step instructions for creating a Machine Learning model using [Teachable Machine by Google](https://teachablemachine.withgoogle.com). It is designed for beginners to get hands-on experience with ML without writing any code.

---

## Table of Contents

1. [Overview](#overview)
2. [Tools & Frameworks Used](#tools--frameworks-used)
3. [Step-by-Step Guide](#step-by-step-guide)
4. [Example Use Cases](#example-use-cases)
5. [Export Options](#export-options)

---

## Overview

**Teachable Machine** is a web-based tool by Google that allows users to create machine learning models quickly and easily using images, sounds, or poses.

---

## Tools & Frameworks Used

### 1. **Teachable Machine**
- A no-code platform to build ML models using transfer learning.
- Supports three types of projects:
  - **Image Project**: Classifies objects or scenes.
  - **Audio Project**: Recognizes sound patterns or voice.
  - **Pose Project**: Detects human body pose or gestures.

### 2. **TensorFlow.js**
- Exported models from Teachable Machine are often in TensorFlow.js format.
- Enables running the trained model directly in the browser using JavaScript.

### 3. **TensorFlow (Python)**
- Teachable Machine also allows downloading the model in `.h5` or `SavedModel` format for use in Python-based ML projects.

### 4. **Webcam / Microphone**
- Input devices for capturing real-time data during training and testing (image/audio projects).

---

## Step-by-Step Guide

### Step 1: Go to Teachable Machine
Visit [https://teachablemachine.withgoogle.com](https://teachablemachine.withgoogle.com)

---

### Step 2: Choose a Project Type
You can choose from:
- **Image Project** – Classify objects, gestures, or environments.
- **Audio Project** – Train your model to detect sounds or spoken words.
- **Pose Project** – Detect body positions for activities like workouts.

---

### Step 3: Create Classes
Define categories for the model to learn.
- Examples: `Cat`, `Dog`, `Bird`
- Provide training data by:
  - Recording through webcam/mic.
  - Uploading image/audio files.

---

### Step 4: Train Your Model
Click **"Train Model"**.
- Uses **transfer learning** with pre-trained models.
- Fast and efficient training process.

---

### Step 5: Test the Model
Test real-time predictions with the input device (e.g., webcam).
- Displays classification results with confidence percentages.

---

### Step 6: Export the Model

Options:
- **TensorFlow.js** – For web-based applications.
- **TensorFlow** – For backend Python ML apps.
- **Coral** – For edge devices (TPU support).

---

## Example Use Cases

- **Gesture recognition** in interactive web apps.
- **Sound detection** for voice commands.
- **Pose analysis** for fitness tracking.
- **Educational tools** for learning ML basics.

---

## Export Options

| Format            | Description                                      | Use Case                      |
|-------------------|--------------------------------------------------|-------------------------------|
| TensorFlow.js     | JavaScript-based model for the web               | Web Applications              |
| TensorFlow        | Python-based model (SavedModel or Keras format) | ML Backend / Python Projects  |
| Coral (Edge TPU)  | Optimized for on-device AI on edge hardware      | IoT / Embedded Systems        |

---

## License & Credits
This guide is based on tools by **Google Teachable Machine** and **TensorFlow**. For educational purposes only.