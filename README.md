# 🛰️ Land Type Classification using Sentinel-2 (EuroSAT)

## 🎓 DEPI Graduation Project

## 📌 Project Overview
This project applies **Deep Learning (CNNs)** to classify different land types using **Sentinel-2 satellite imagery** from the European Space Agency.  
The goal is to build a model capable of distinguishing between multiple land-use categories including:

- 🌾 Annual Crop  
- 🌳 Forest  
- 🌿 Herbaceous Vegetation  
- 🏙️ Residential  
- 🏭 Industrial  
- 🛣️ Highway  
- 🐄 Pasture  
- 🍇 Permanent Crop  
- 🏞️ River  
- 🌊 Sea / Lake  

These predictions support real-world applications such as **urban planning, environmental monitoring, agricultural analysis, and resource management**, providing accurate land-use classification insights.

---

## 📊 Dataset
- The project uses the **EuroSAT Sentinel-2 dataset** (~27k images).  
- Images are **64×64 RGB** (multispectral available).  
- Contains **10 balanced classes** representing different land-cover types.  
- Sentinel-2’s multispectral capabilities make it ideal for geospatial classification tasks.

---

## 🛠 Tools & Libraries
The following tools and libraries were used for image processing, model training, and evaluation:

- **Pandas** 🐼 – Data handling  
- **NumPy** 🔢 – Numerical operations  
- **os** 📂 – File management  
- **cv2** 📸 – Image preprocessing  
- **Matplotlib / Seaborn** 📊 – Data visualization  
- **TensorFlow / Keras** 🤖 – Deep Learning framework  
- **scikit-learn** – Metrics & evaluation utilities  

---

## 🚀 Project Workflow

### 1. **Data Collection & Preprocessing**
- Load EuroSAT dataset.  
- Resize, normalize, and prepare image tensors.  
- Apply augmentation (rotation, zoom, flipping, brightness).  
- Split into training & validation sets.

### 2. **Exploratory Data Analysis (EDA)**
- Visualize class distribution.  
- Display sample images from each category.  
- Inspect RGB histograms and pixel intensity profiles.  
- Analyze dataset balance and visual consistency.

### 3. **Model Development**
- Build a **Convolutional Neural Network** using TensorFlow/Keras:  
  - Rescaling + RandomAugmentation layers  
  - Conv2D → BatchNorm → MaxPooling blocks  
  - GlobalAveragePooling  
  - Dense(512) + Dropout  
  - Softmax output (10 classes)  
- Train using Adam optimizer & categorical crossentropy.  
- Apply callbacks: EarlyStopping, ReduceLROnPlateau, ModelCheckpoint.

### 4. **Deployment & Results Interpretation**
- Evaluate using accuracy, loss curves, and confusion matrix.  
- Test the model on unseen satellite images.  
- Visualize predictions & interpret classification behavior.

---

## 🔗 Conclusion
Through the integration of **Deep Learning and Sentinel-2 imagery**, this project delivers effective **land-type classification**, supporting applications such as:  
- 🌱 Crop monitoring  
- 🌍 Environmental analysis  
- 🌳 Deforestation tracking  
- 🚨 Disaster response  
- 🏙️ Urban development planning  

The model demonstrates strong performance and provides valuable geospatial insights for real-world decision-making.

---

🔗 **Analyze Land. Classify Smart. Transform Insights into Actions.**
