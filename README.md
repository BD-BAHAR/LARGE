
# Look-Alike Medical Vial Detection Using YOLOv4-Tiny

This repository demonstrates the detection of look-alike medical vials, a critical application in the healthcare industry, using the YOLOv4-Tiny deep learning model. The solution is optimized for real-time vial detection, addressing the challenges of distinguishing similar-looking vials to prevent medication errors.

## Features

- **Deep Learning**: Utilizes YOLOv4-Tiny for efficient object detection.
- **Custom Dataset**: Trains a model using a labeled dataset specific to medical vials.
- **Real-Time Detection**: Supports inference on images, videos, and live webcam feeds.
- **Custom Configuration**: Includes custom YOLO configuration for optimized training.

## Requirements

- Google Colab or a local machine with GPU support.
- Required libraries: TensorFlow, OpenCV, and Darknet.
- A labeled dataset of medical vials.

## Steps to Use

### 1. Setup Environment
- Clone the Darknet repository and set up the YOLOv4-Tiny environment in Google Colab or on your local machine.
- Enable GPU for faster training and inference.

### 2. Prepare Dataset
- Upload a labeled dataset (`obj.zip`) with annotations in YOLO format.
- Use the `process.py` script to divide the dataset into training and testing sets.

### 3. Configure YOLOv4-Tiny
- Modify the YOLOv4-Tiny configuration file:
  - Adjust parameters like `batch`, `subdivisions`, and `max_batches`.
  - Set the number of classes and filters to match the dataset.

### 4. Training
- Train the model using the pre-trained YOLOv4-Tiny weights.
- Save checkpoints during training to resume if interrupted.

### 5. Evaluate and Test
- Validate the model's performance using mAP (mean Average Precision).
- Test the trained model on images, videos, and live webcam feeds.

## File Structure

- **Notebook**: The main `.ipynb` file containing all steps for training and inference.
- **Custom Files**: Includes configuration files, `obj.data`, `obj.names`, and the `process.py` script.
- **Data**: Folder for storing labeled dataset and generated `train.txt` and `test.txt` files.

## Results

- Real-time detection of look-alike vials with high accuracy.
- Performance metrics such as mAP, precision, and recall provided after training.


