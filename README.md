
# 🩺 Kidney Disease Classification using Vision Transformers and Explainable AI

## 📌 Problem Statement  
Kidney abnormalities such as cysts, stones, and tumors are difficult to detect manually in CT scans due to subtle variations in visual patterns. Manual analysis by radiologists is time-consuming, error-prone, and lacks consistency.  
This project aims to build an **accurate, reliable, and explainable AI-based system** for automatic kidney disease classification.

---

## 🚀 Approach  
1. **Dataset Preparation**  
   - Used **CT-Kidney Dataset** with **12,000+ CT images** across four categories: *Normal, Cyst, Stone, Tumor*.  
   - Preprocessing included **resizing (128×128)**, normalization, and **augmentation** (rotation, flipping, zoom, brightness).  

2. **Model Development**  
   - Implemented **transfer learning** with:  
     - **Vision Transformer (ViT)**  
     - **ResNet50**  
     - **VGG16**  
   - Optimized using **categorical cross-entropy loss** and **Adam optimizer**.  
   - Applied **Early Stopping** and **Checkpointing** to prevent overfitting.  

3. **Explainability**  
   - Integrated **Grad-CAM** to generate heatmaps highlighting regions contributing to predictions for better **clinical interpretability**.  

---

## 📊 Results  

| Model                | Accuracy | Precision | Recall | F1-Score |
|-----------------------|---------|-----------|--------|----------|
| Vision Transformer    | 96.37%   | 95.86%   | 95.24% | 95.55%   |
| ResNet50              | 94.26%   | 93.73%   | 92.81% | 93.27%   |
| VGG16                 | 92.85%   | 92.85%   | 90.71% | 91.06%   |

✅ **Vision Transformer outperformed CNN-based models** by effectively capturing **global spatial dependencies**.  
✅ **Grad-CAM** added **explainability**, building trust in clinical decision-making.  

---

## 🛠 Tech Stack  
- **Programming:** Python  
- **Frameworks:** TensorFlow, Keras  
- **Models:** Vision Transformer (ViT), ResNet50, VGG16  
- **Explainability:** Grad-CAM  
- **Libraries:** NumPy, Pandas, Matplotlib, OpenCV  
- **Optimization:** Adam, Early Stopping, Checkpointing  
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score  

