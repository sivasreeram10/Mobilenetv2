# MobileNetV2-Based Banana Plant Disease Detection  

## Overview  
This project implements **MobileNetV2**, a lightweight and efficient deep learning model, for detecting banana plant diseases using leaf images. The model is optimized for **mobile and edge devices**, making real-time disease detection possible without heavy computational requirements.  

## Features  
✅ **Lightweight & Fast** – MobileNetV2 reduces computation while maintaining high accuracy.  
✅ **Optimized for Mobile & Edge Devices** – Runs efficiently on smartphones and IoT devices.  
✅ **Real-Time Disease Detection** – Classifies banana leaf diseases in seconds.  
✅ **Uses Transfer Learning** – Leverages the power of a **pretrained ImageNet** model.  

## Dataset  
The model is trained on a dataset containing **healthy and diseased banana leaf images**. Categories include:  
- **Healthy Leaves**  
- **Diseased Leaves** (e.g., Black Sigatoka, Fusarium Wilt, Banana Bunchy Top Virus, etc.)  

## Workflow  
### **1. Data Preprocessing**  
- Load high-resolution banana leaf images.  
- Resize images to **224×224 pixels** (MobileNetV2 input size).  
- Apply **image augmentation** (rotation, flipping, contrast adjustment) for improved generalization.  

### **2. Model Architecture (MobileNetV2)**  
MobileNetV2 enhances feature extraction by using:  
- **Depthwise Separable Convolutions** – Reduces computation without losing accuracy.  
- **Inverted Residual Blocks** – Improves feature reuse and efficiency.  
- **Batch Normalization** – Stabilizes and speeds up training.  

### **3. Training the Model**  
- **Loss Function**: Categorical Cross-Entropy  
- **Optimizer**: Adam (Adaptive Learning Rate)  
- **Evaluation Metrics**: Accuracy & Loss on Training/Validation Set  

### **4. Classification & Prediction**  
- The trained model classifies banana leaf images into **healthy or diseased** categories.  
- Provides **confidence scores** for predictions.  
- Can be deployed on **mobile apps, web platforms, and IoT-based monitoring systems**.  

## Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/mobilenetv2-banana-disease-detection.git
   cd mobilenetv2-banana-disease-detection
Install dependencies:
bash
Copy
Edit
pip install -r requirements.txt
Train the model:
bash
Copy
Edit
python train.py
Run inference on a sample image:
bash
Copy
Edit
python predict.py --image sample_leaf.jpg
Results
Achieved high accuracy in detecting banana plant diseases.
Faster inference time compared to other CNN-based models.
Future Improvements
🔹 Expand dataset for better generalization.
🔹 Optimize for real-time edge computing applications.
🔹 Integrate with IoT-based disease monitoring systems for farmers.
