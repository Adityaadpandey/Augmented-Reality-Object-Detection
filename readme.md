# Augmented Reality Project

This folder contains an Augmented Reality (AR) application that performs real-time object detection using a pre-trained MobileNet-SSD model. The project uses Python 3.6, and it’s recommended to run it in an Anaconda environment.

## Requirements

1. **Python Version**: Python 3.6 (recommended via Anaconda)
2. **Dependencies**: Install the required packages by running:

   ```bash
   pip install -r requirements.txt
   ```

## Running the AR Application

After installing the necessary dependencies, you can run the object detection code to enable real-time object detection in an AR environment.

### Instructions for Running

1. **Linux/MacOS**:

   ```bash
   python3 real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
   ```

2. **Windows**:

   ```bash
   python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
   ```

## Files

- `real_time_object_detection.py`: The main script for running the object detection model in real-time.
- `MobileNetSSD_deploy.prototxt.txt`: The configuration file defining the MobileNet-SSD model structure.
- `MobileNetSSD_deploy.caffemodel`: The pre-trained MobileNet-SSD model weights.

## Description

The application uses a MobileNet-SSD model to detect objects in real-time through a connected camera or video feed. The detected objects are overlaid with bounding boxes, making it suitable for augmented reality applications.

## Notes

- Ensure that your camera is properly connected for real-time detection.
- Adjust the detection threshold in the script if necessary to improve accuracy or speed.
