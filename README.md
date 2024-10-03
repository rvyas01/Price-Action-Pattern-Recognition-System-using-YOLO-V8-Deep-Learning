Price Action Pattern Recognition using Candlestick Chart Images
This project focuses on recognizing price action patterns from candlestick chart images using YOLO-V8 and computer vision techniques. It involves dataset creation, annotation, and model training to detect financial patterns effectively.

Project Overview
Project Link: Roboflow Project - Stock Pattern Recognition
Created by: Rishi Vyas
Date: March 2024
Key Features
Dataset Creation: I developed a custom dataset of 400 financial candlestick chart images from scratch.
Annotation: The dataset was 100% annotated by myself using Roboflow and Python.
Model: Utilized YOLO-V8 for detecting complex price action patterns.
Performance: Achieved a precision rate of 60%, with additional improvements through data augmentation techniques.
Dataset
Structure
The dataset is organized as follows:

plaintext
Copy code
📂 data
    ├── README.dataset (1 KB)
    ├── README.roboflow (2 KB)
    ├── valid/
    ├── train/
    ├── test/
Each of the train, valid, and test folders contains two subdirectories:

plaintext
Copy code
📂 train/
    ├── images/
    └── labels/
    
📂 valid/
    ├── images/
    └── labels/
    
📂 test/
    ├── images/
    └── labels/
images/: Contains the candlestick chart images used for training, validation, and testing.
labels/: Contains the YOLO format .txt files with corresponding annotations for the images.
Download Dataset
You can download the dataset from my Roboflow project page:
Stock Pattern Recognition Dataset

How to Use the Model
Installation
To test this model on your own system, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/price-action-recognition.git
cd price-action-recognition
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Download the dataset: Follow the instructions in the Dataset section to download and place the dataset in the appropriate directory.

Run the YOLO-V8 model: Ensure you have YOLO-V8 installed, and then run the model using:

bash
Copy code
python detect.py --source data/test --weights best.pt --conf 0.25
--source: Path to your test dataset.
--weights: Path to the YOLO-V8 trained model weights.
--conf: Confidence threshold for predictions.
Visualize results: Once the detection is complete, the output images will be stored in the /output directory with bounding boxes drawn around the detected patterns.

Model Evaluation
Precision: 60%
Data Augmentation: Applied to improve accuracy.
YOLO-V8: Utilized for high-performance pattern detection.
Tools and Technologies
Roboflow: Used for dataset annotation and preprocessing.
YOLO-V8: Object detection model for pattern recognition.
Python: For automating data handling and running the model.
Machine Learning: Used to train the model to detect price action patterns.
Conclusion
This project leverages machine learning and computer vision to improve financial market analysis through automated pattern recognition in candlestick charts. The use of a custom dataset and YOLO-V8 enables robust detection of complex price patterns, aiding in financial decision-making.

