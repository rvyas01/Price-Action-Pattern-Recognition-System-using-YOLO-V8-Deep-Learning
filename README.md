
# 📊 Price Action Pattern Recognition using Candlestick Chart Images

This project leverages **YOLO-V8** and **machine learning** to detect price action patterns from financial candlestick charts, enhancing market analysis through automated pattern recognition.

## 🚀 Project Overview

- **Project Link**: [Roboflow Project - Stock Pattern Recognition](https://universe.roboflow.com/rishi-vyas-vbwyc/stock-pattern-recognition/dataset/2)
- **Date**: March 2024
- **Author**: Rishi Vyas

### 🔑 Key Features

- **Dataset**: Custom-created with 400 financial candlestick chart images, fully annotated by me using **Roboflow** and **Python**.
- **Model**: Trained with **YOLO-V8** to detect complex price patterns.
- **Performance**: Achieved 60% precision, further improved using **data augmentation**.

---

## 📂 Dataset Structure

```plaintext
📦 data/
 ┣ 📜 README.dataset  
 ┣ 📜 README.roboflow  
 ┣ 📂 train/  
 ┃ ┣ 📂 images/  
 ┃ ┣ 📂 labels/  
 ┣ 📂 valid/  
 ┃ ┣ 📂 images/  
 ┃ ┣ 📂 labels/  
 ┣ 📂 test/  
 ┃ ┣ 📂 images/  
 ┃ ┣ 📂 labels/  
```

- **images/**: Contains candlestick chart images for training, validation, and testing.
- **labels/**: Contains YOLO format `.txt` files with annotations corresponding to each image.

### Download Dataset

You can download the dataset directly from my [Roboflow Project Page](https://universe.roboflow.com/rishi-vyas-vbwyc/stock-pattern-recognition/dataset/2).

---

## 🛠️ How to Use the Model

### 1. Clone the Repository

```bash
git clone https://github.com/your-repo/price-action-recognition.git
cd price-action-recognition
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download and Place Dataset

Follow the instructions in the [Dataset](#dataset-structure) section to download and place the dataset in the appropriate directory.

### 4. Run YOLO-V8 Model

Make sure YOLO-V8 is installed and execute the following:

```bash
python detect.py --source data/test --weights best.pt --conf 0.25
```

- `--source`: Path to the test dataset.
- `--weights`: Path to the YOLO-V8 model weights.
- `--conf`: Confidence threshold for predictions.

### 5. Visualize Results

Output images with bounding boxes will be saved in the `/output` directory, showing detected price action patterns.

---

## 🔍 Model Evaluation

- **Precision**: 60%
- **Techniques**: Data augmentation used to boost accuracy.
- **Detection Model**: YOLO-V8 for high-performance pattern detection.

---

## 🛠️ Tools and Technologies

- **Roboflow**: For dataset annotation and preprocessing.
- **YOLO-V8**: Object detection framework for pattern recognition.
- **Python**: Automation, data handling, and model execution.
- **Machine Learning**: Training for pattern detection.

---

## 📈 Conclusion

This project demonstrates the power of machine learning and computer vision in the financial sector by automating price pattern recognition in candlestick charts. The use of **YOLO-V8** and custom datasets enables efficient and accurate pattern detection to support financial decision-making.
