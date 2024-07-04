# CodeAlfa_project
# Face Recognition with YOLOv5

This repository contains the code and instructions for a face recognition project using the YOLOv5 model. The model is trained to recognize my face using a custom dataset.

## Project Overview

- **Model**: YOLOv5
- **Task**: Face Recognition
- **Data**: Custom dataset (not provided due to privacy reasons)

## Getting Started

### Prerequisites

- Python 3.8 or later
- [YOLOv5](https://github.com/ultralytics/yolov5)
- Other dependencies listed in `requirements.txt`

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/face-recognition-yolov5.git
    cd face-recognition-yolov5
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. **Training the Model**:
    - Ensure you have your data in the appropriate format.
    - Modify the `data.yaml` file to include your dataset paths and classes.
    - Train the model using:
      ```bash
      python train.py --img 640 --batch 16 --epochs 100 --data data.yaml --cfg models/yolov5s.yaml --weights yolov5s.pt
      ```

2. **Inference**:
    - Run the inference script to test the model on new images:
      ```bash
      python detect.py --weights runs/train/exp/weights/best.pt --img 640 --source path/to/your/image.jpg
      ```

## Results

The model was able to successfully recognize my face with high accuracy. Below are some example results:

![Example 1](example1.jpg)
![Example 2](example2.jpg)

## Acknowledgments

- [YOLOv5 by Ultralytics](https://github.com/ultralytics/yolov5)
- All the open-source libraries used in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
