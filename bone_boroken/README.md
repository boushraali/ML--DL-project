# 🦴 Bone Fracture Detection using MobileNet

The **medical field** is one of the most prominent domains that has greatly benefited from **Artificial Intelligence**, especially in **medical image analysis**.  
In this research-based experiment, a **MobileNet** model was applied to detect **bone fractures**, using the **Bone Fracture Multi-Region X-ray** dataset available on **Kaggle**.

---

## ⚙️ Experiment Workflow

1. **Data Augmentation**  
   Enhanced the training dataset with augmentation techniques to improve model generalization and robustness.

2. **Pre-trained Model & Fine-Tuning**  
   Utilized **MobileNet** as a pre-trained model and applied **fine-tuning** by modifying the final layers:
   - `GlobalAveragePooling2D`  
   - `Dense layer`  
   - `Dropout(0.5)` to reduce overfitting  
   - Final `Dense` layer for classification  

3. **Regularization & Optimization**  
   Applied:
   - **EarlyStopping** to avoid overtraining when validation accuracy stops improving  
   - **ReduceLROnPlateau** to dynamically adjust the learning rate  

4. **Interactive Interface (Streamlit)**  
   Designed a **Streamlit** web interface allowing users to upload X-ray images and test the model’s predictions.  
   The app was connected via **pyngrok** for live model testing on real data.

---

## 📊 Test Results

| Metric | Value |
|--------|--------|
| ✅ Test Accuracy | **0.9506** |
| ✅ Test AUC | **0.9858** |

These results indicate a strong model performance with excellent discrimination between normal and fractured bone X-rays.

---

## 🎥 Demo Video
Watch the full demonstration of the project here:  
[▶️ Watch Demo on Google Drive](https://drive.google.com/file/d/1vB__RPtdbuvk4OoPxgXFuflbVmIwy5ic/view?usp=sharing)

The demo showcases:
- Data preprocessing and model training  
- Streamlit interactive interface  
- Real-time predictions on X-ray images  

---

## 🧠 Tools & Technologies
- **Python**
- **TensorFlow / Keras**
- **NumPy, Pandas, Matplotlib**
- **Streamlit**
- **pyngrok**
- **Kaggle Dataset: Bone Fracture Multi-Region X-ray**

---

## 💡 Future Work
- Experiment with deeper architectures such as **EfficientNet** or **DenseNet**.  
- Apply **Explainable AI (Grad-CAM)** to visualize model attention on fracture areas.  
- Build a **Streamlit dashboard** for doctors to analyze uploaded X-ray scans interactively.  
