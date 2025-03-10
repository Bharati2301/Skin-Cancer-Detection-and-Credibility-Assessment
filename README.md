## 🩺 Detection of Skin Cancer & Credibility Assessment using Explainable AI

### 📌 Overview

Skin cancer is one of the most prevalent and dangerous types of cancer worldwide. This project leverages **Deep Learning** and **Explainable AI (XAI)** techniques to build an advanced skin cancer detection system. Using **SHapley Additive exPlanations (SHAP)**, we enhance model transparency and credibility, aiding medical professionals in decision-making. 

🔬 **Key Features:**
- **ResNet50-based** deep learning model for **skin cancer classification**.
- Uses **SHAP** for model interpretability and credibility assessment.
- Trained on the **SIIM-ISIC** dataset with images and metadata (age, gender, etc.).
- **Early detection** to improve treatment outcomes and save lives.
- Compares multiple models (**CNN, VGG16, InceptionResNetV2, ResNet50**).

---

## 🔍 Methodology

1️⃣ **Data Preprocessing** 🪚  
   - Dataset cleaning, balancing, and augmentation using **ImageDataGenerator**.  
   - Standardized input scaling (128x128 resolution).  

2️⃣ **Model Training** 🏋️  
   - Tested **CNN, VGG16, InceptionResNetV2, and ResNet50**.  
   - **ResNet50** selected as best performer due to stability and high **AUC-ROC**.  

3️⃣ **SHAP-based Explainability** 📊  
   - Highlights important features in images influencing the model’s decision.  
   - **Pink = high impact regions, Blue = low impact regions** in classification.  

4️⃣ **Performance Metrics** 📈  
   - **Accuracy, Recall, AUC-ROC, Loss Analysis**.  
   - ResNet50 achieved **highest stability and credibility**.  

---

## 📊 Results

| Model | Accuracy | AUC-ROC | Recall |
|--------|---------|--------|--------|
| CNN | 91.70% | 91.93% | 53.87% |
| **VGG16** | **93.64%** | **94.73%** | **82.41%** |
| InceptionResNetV2 | 92.52% | 91.93% | 65.60% |
| **ResNet50 (Best)** | **90.21%** | **91.09%** | **38.55%** |

**🔹 ResNet50** was the most stable model with **high credibility** when tested using **SHAP analysis**.

---

## 📌 Future Enhancements

🔹 **Continuous model updates** with real-world data.  
🔹 **Advanced augmentation techniques** for better dataset diversity.  
🔹 **Ensemble learning** for even higher accuracy.  

---

## 🏆 Acknowledgments

- **SIIM-ISIC** dataset contributors.
- **Kaggle & TensorFlow** for model references.
- **SHAP** library for Explainable AI.
