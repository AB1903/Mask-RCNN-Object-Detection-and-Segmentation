# Mask-RCNN Object Detection and Segmentation

This repository implements Mask-RCNN for object detection and instance segmentation using OpenCV's Deep Neural Network (DNN) module. The project processes images and videos to detect objects, draw bounding boxes, and apply segmentation masks.

---

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Model Files](#model-files)
- [Arguments](#arguments)
- [Output](#output)
- [Contributing](#contributing)

---

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mask-rcnn-object-detection.git
    ```
2. Navigate to the project directory:
    ```bash
    cd mask-rcnn-object-detection
    ```
3. Install the required dependencies:
    ```bash
    pip install opencv-python numpy
    ```

---

## Usage
1. **Running on an Image:**
   To run the Mask-RCNN model on an image:
    ```bash
    python mask_rcnn.py --image /path/to/image.jpg --device cpu
    ```

2. **Running on a Video:**
   To run the Mask-RCNN model on a video:
    ```bash
    python mask_rcnn.py --video /path/to/video.mp4 --device gpu
    ```

3. **Running on a Webcam:**
   To run the Mask-RCNN model on your webcam:
    ```bash
    python mask_rcnn.py --device cpu
    ```

---

## Features
- **Object Detection and Segmentation:** Uses Mask-RCNN for real-time object detection and segmentation.
- **Device Selection:** Runs inference on either CPU or GPU.
- **Output:** Saves processed results as an image or video and displays real-time detection.
- **Compatibility:** Supports both images and videos as inputs.

---

## Model Files
The following model files are required:
- `mscoco_labels.names` (Contains class labels)
- `mask_rcnn_inception_v2_coco_2018_01_28.pbtxt` (Text graph file for the model)
- `frozen_inference_graph.pb` (Pre-trained model weights)
- `colors.txt` (Predefined colors for object masks)

Ensure these files are in the same directory as the script.

---

## Arguments
- `--image` : Path to the input image file.
- `--video` : Path to the input video file.
- `--device` : Specify `cpu` or `gpu` for inference.

---

## Output
- Processed images will be saved as `<input_name>_mask_rcnn_out_py.jpg`
- Processed videos will be saved as `<input_name>_mask_rcnn_out_py.mp4`
- The detection results will be displayed in a window.

---

## Contributing
Feel free to open issues or create pull requests to improve this project. Contributions are always welcome!

---
