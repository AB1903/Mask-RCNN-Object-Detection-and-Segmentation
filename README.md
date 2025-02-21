##Mask-RCNN Object Detection and Segmentation##

Overview

This project implements Mask-RCNN for object detection and instance segmentation using OpenCV's Deep Neural Network (DNN) module. The script can process images and videos to detect objects, draw bounding boxes, and apply segmentation masks.

Features

Object detection and segmentation using Mask-RCNN

Supports both image and video input

Runs inference on CPU or GPU

Saves processed output as an image or video

Displays real-time detection results

Prerequisites

Ensure you have the following installed before running the script:

Python 3.x

OpenCV (cv2)

NumPy

You can install dependencies using:

pip install opencv-python numpy

Installation

Clone the repository:

git clone https://github.com/yourusername/mask-rcnn-object-detection.git
cd mask-rcnn-object-detection

Usage

Running on an Image

python mask_rcnn.py --image /path/to/image.jpg --device cpu

Running on a Video

python mask_rcnn.py --video /path/to/video.mp4 --device gpu

Running on a Webcam

python mask_rcnn.py --device cpu

Arguments

--image : Path to the input image file.

--video : Path to the input video file.

--device : Specify cpu or gpu for inference.

Model Files

The following model files are required:

mscoco_labels.names (contains class labels)

mask_rcnn_inception_v2_coco_2018_01_28.pbtxt (text graph file for the model)

frozen_inference_graph.pb (pre-trained model weights)

colors.txt (predefined colors for object masks)

Ensure these files are in the same directory as the script.

Output

Processed images will be saved as <input_name>_mask_rcnn_out_py.jpg

Processed videos will be saved as <input_name>_mask_rcnn_out_py.mp4

The detection results will also be displayed in a window.

Contributing

Feel free to contribute to the project by submitting issues or pull requests.

License

This project is open-source and available under the MIT License.

Contact

For any inquiries, reach out via email or create an issue on GitHub.

Show Some ❤️ by Starring the Repository!

If you find this project useful, please consider giving it a ⭐ on GitHub!


