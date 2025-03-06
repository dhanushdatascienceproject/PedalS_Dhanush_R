COLAB LINK: https://colab.research.google.com/drive/1yr18HIaHRmk5NhowgBvRNRODqGzl87hD?usp=sharing

GENERATED IMAGES:

![Image](https://github.com/user-attachments/assets/737b9f55-4584-481f-815a-265d61711dac)

![Image](https://github.com/user-attachments/assets/807fa213-a979-4fc7-a69c-f55a577752c0)

![Image](https://github.com/user-attachments/assets/8f803976-6101-446e-b499-5bf9a4963eef)

![Image](https://github.com/user-attachments/assets/13a239d2-e580-435e-aba4-99109409ae2b)




PREPROCESSED IMAGES:

![preprocessed_image_2 (1)](https://github.com/user-attachments/assets/ff25a38a-2d6e-49c7-be50-5940d97fd285)


![preprocessed_image_1](https://github.com/user-attachments/assets/3e1ed374-ae7f-48f2-8de3-3ff04a40cbf1)
![preprocessed_image_3](https://github.com/user-attachments/assets/ae733ac2-9c2c-4a74-89c6-683dc8ecdcbb)

# Image Generation & Classification using Flux (Julia) & Python

## 📌 Project Overview
This project focuses on **image generation and preprocessing using Python** and **image classification using Flux (Julia)**. The workflow includes:

1. **Generating realistic high-resolution images** using Python.
2. **Preprocessing the images** (resizing, normalization, format conversion).
3. **Building a CNN-based classification model** in Julia with the Flux framework.
4. **Testing the model with preprocessed images** and predicting the class.

---

## 🚀 How to Set Up Your Environment

### **🔧 Prerequisites**
- **Google Colab** (for running Python scripts)
- **Julia 1.x** (with Flux.jl installed)
- **GitHub or Google Drive** (for submission)

### **📌 Installation Steps**
#### **1️⃣ Setting Up Julia in Colab**
```sh
!apt update && apt install -y julia
```
#### **2️⃣ Installing Required Julia Packages**
```julia
using Pkg
Pkg.add(["Flux", "Images", "ImageTransformations", "FileIO"])
```
#### **3️⃣ Installing Required Python Libraries**
```python
!pip install pillow numpy matplotlib opencv-python
```

---

## 📂 Project Structure
```
📦 Project Folder
 ├── 📜 generate_images.py         # Python script to generate images
 ├── 📜 preprocess_images.py       # Python script for image preprocessing
 ├── 📜 model.jl                   # Julia script for CNN classification
 ├── 📜 requirements.txt           # Dependencies list
 ├── 📜 README.md                  # Documentation (this file)
 ├── 📂 images                      # Folder containing generated images
 ├── 📂 preprocessed_images         # Folder containing preprocessed images
```

---

## 📌 Image Generation & Preprocessing (Python)
### **Step 1: Generate High-Resolution Images**
Run the Python script to generate synthetic high-resolution images:
```sh
python generate_images.py
```

### **Step 2: Preprocess Images**
Resize and normalize images before passing them to the model:
```sh
python preprocess_images.py
```

---

## 📌 Image Classification (Flux in Julia)
### **Step 3: Run the Julia Model**
Run the Flux-based CNN model on a preprocessed image:
```sh
julia model.jl
```

### **Step 4: Model Output & Prediction**
The script will output the predicted class:
```
Model Output: [0.08, 0.1, 0.09, ..., 0.11]
Predicted Class: 9
```

---

## 📌 Challenges & Assumptions
### **Challenges Faced**
- Handling **high-resolution images** in memory.
- Understanding the **Flux.jl API** for CNNs.
- Fixing `softmax` and `flatten` function errors.

### **Assumptions**
- The dataset contains **10 classes** for classification.
- The generated images resemble real-world objects.

---

## 📌 Submission Instructions
### **🔹 Option 1: Upload ZIP to Google Drive**
1. Zip all project files:
   ```sh
   zip -r project.zip *
   ```
2. Move ZIP file to Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   !mv /content/project.zip /content/drive/MyDrive/
   ```

### **🔹 Option 2: Upload to GitHub**
1. Initialize a Git repository and push your files:
   ```sh
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

### **🔹 Option 3: Direct Download**
```python
from google.colab import files
files.download('/content/project.zip')
```

---

## 🎯 Conclusion
This project demonstrates the end-to-end workflow of **image generation, preprocessing, and classification** using **Python & Julia**. 🚀
