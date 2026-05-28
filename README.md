# Project Overview

This project explores real-time interpersonal interaction using computer vision and audio-visual synthesis.

The system integrates:

* YOLOv8 for object detection and spatial analysis
* Max/MSP for real-time audio-visual interaction

Collaborated with Martijn Bernard Straatsburg.

## System Pipeline

1. Input (camera / video)
2. YOLOv8 performs detection and extracts spatial data
3. Processed data is sent to Max/MSP
4. Max/MSP generates interactive sound / visual output

---

## Base Model

This project is based on YOLOv8 Webcam Object Detection developed by:
https://github.com/codershiyar/object-detection-using-webcam.git
And and incorporates additional code provided by the course instructor, Maurizio Berta, as part of the teaching materials.
We acknowledge and thank the instructor for the guidance and foundational implementation support.

## Modifications

The following modifications were made to the original YOLOv8 implementation：

* Customized model architecture for computing proximity
* Modified data preprocessing pipeline
* Added interface for real-time data output to Max/MSP

---

## Max/MSP Integration

The Max/MSP patch receives detection data and maps it to interactive audio/visual outputs.

---

## Notes

Only modified YOLO components are included in this repository.
Please clone the original YOLOv8 repository and integrate the provided files.

---

## Reproducibility

1. Clone YOLOv8:
   git clone https://github.com/codershiyar/object-detection-using-webcam.git

2. Replace relevant files with those in `yolo_mod/`

3. Run YOLO inference

4. Open the Max/MSP patch and connect to the data stream
