![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![Intel oneAPI](https://img.shields.io/badge/Intel-oneAPI-blue)

# ExplainCrop AI

ExplainCrop AI is an intelligent computer vision system designed to identify plants and weeds from images and provide actionable agricultural insights.

This project leverages deep learning with transfer learning (MobileNetV2) to classify plant species such as **Celosia Argentea**, **Crowfoot Grass**, and **Purple Chloris**. Beyond classification, the system integrates Explainable AI (Grad-CAM) to visually justify predictions and a smart advisory layer to guide user decisions.

---

## Features

*  Image-based plant & weed classification
*  Transfer learning using MobileNetV2
*  Explainable AI with Grad-CAM visualization
*  Smart advisory system (risk level + recommended action)
*  Optimized data pipeline for efficient training

---

## How It Works

1. User uploads an image
2. Model predicts plant/weed class
3. System determines:

   * Type (Weed / Useful Plant)
   * Risk level
   * Recommended action
4. Grad-CAM highlights regions responsible for prediction

---

## Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Intel oneAPI (oneDNN, oneDAL via sklearnex)

---
## Intel oneAPI Optimization
This project leverages Intel oneAPI optimizations for improved performance:

- TensorFlow uses Intel oneDNN for accelerated deep learning operations
- Scikit-learn is optimized using Intel oneDAL via sklearnex
---
## Sample Output

*  Prediction with confidence score
*  Risk level (Low / High)
*  Action recommendation
*  Visual explanation (heatmap)
  
<h3> Sample Input</h3>
<img src="results/input_img.jpeg" width="400">
<h3> Prediction Output</h3>
<img src="results/prediction.png">
<h3> Grad-CAM Explanation</h3>
<img src="results/gradcam.png" width="400">
The highlighted regions show the parts of the image the model focused on for prediction.

---
## Model Performance
Achieved over 95% accuracy on validation dataset with strong classification performance.

## Objective

To assist users and farmers in identifying harmful weeds and making informed decisions using AI-powered insights and explainable predictions.

---

## Note

* This project is developed and tested using **Google Colab**
* Some upload-related code (e.g., `files.upload()`) works only in Colab environment

---

## Installation

```bash
pip install tensorflow opencv-python numpy matplotlib scikit-learn-intelex
```
## How to Run
1. Open the notebook in Google Colab  
2. Install dependencies   
3. Upload the dataset zip file  
4. Provide a test image path (e.g., `/content/test.jpg`)  
5. Run all cells sequentially 

## Future Improvements

* Expand dataset for better generalization
* Deploy as a web/mobile application
* Add real-time detection using camera input

---

## Key Highlight

This project goes beyond basic classification by combining:

- Deep Learning + Explainable AI (Grad-CAM)
- Provides actionable agricultural insights
- Uses Intel oneAPI optimizations for high performance
---

 *ExplainCrop AI demonstrates how AI can move from prediction to meaningful real-world impact.*
