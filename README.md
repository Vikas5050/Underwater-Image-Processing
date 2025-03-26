# 🌊 Underwater Image Processing

This repository contains various methods for enhancing underwater images, developed as part of a project at the **National Institute of Technology** from **January 2024 to June 2024**. The project was conducted by **Vikas**, **Shahbaj**, and **Purushottam** under the guidance of **Dr. Bambam** and **Dr. Ashish Kumar Bhandari**.

---

## 📌 Project Overview

Underwater images often suffer from:

- 🎨 **Color Distortion** – Due to selective absorption of light.
- 🌫️ **Low Visibility & Haze** – Caused by scattering in water.
- 📉 **Reduced Contrast** – Due to light attenuation.

**Goal**: To enhance underwater images using state-of-the-art image processing techniques for better clarity and visualization.

### 🎯 Objectives

- Improve image quality through various enhancement methods.
- Compare traditional methods with advanced techniques.
- Create a modular and extensible codebase for future research.
- Provide clear visual outputs for each enhancement technique.

---

## 🛠️ Implemented Methods

| 📚 Method                           | 📝 Description                                                                 |
|------------------------------------|------------------------------------------------------------------------------|
| 🔍 **CLAHE**                       | Enhances contrast using adaptive histogram equalization with contrast limiting|
| 🌑 **Dark Channel Prior (DCP)**    | Removes haze by estimating the transmission map                               |
| 📊 **HE & DCP**                    | Combines Histogram Equalization and Dark Channel Prior for better dehazing    |
| 🔥 **Fusion-Based Enhancement**     | Fuses multiple images to improve color and visibility                         |
| 💡 **Retinex Method**               | Enhances images by separating illumination and reflectance components         |

### 📊 Methodology

Each method applies a unique approach to improving underwater images:

1. **CLAHE (Contrast Limited Adaptive Histogram Equalization)**
   - Enhances local contrast in small regions.
   - Limits noise amplification by capping the contrast.

2. **Dark Channel Prior (DCP)**
   - Estimates haze by analyzing dark pixels in a local patch.
   - Recovers clear images using a transmission map.

3. **Histogram Equalization & DCP**
   - Applies histogram equalization to improve global contrast.
   - Uses the dark channel prior for local dehazing.

4. **Fusion-Based Enhancement**
   - Blends multiple images to correct color and improve visibility.
   - Uses weight maps to highlight the best features of each image.

5. **Retinex Method**
   - Decomposes the image into illumination and reflectance.
   - Enhances visibility by adjusting reflectance.

---

## 📁 Repository Structure

```
Underwater-Image-Processing/
├── CLAHE.ipynb                # CLAHE Enhancement
├── DCP.ipynb                  # Dark Channel Prior
├── HE&DCP.ipynb               # Combined Histogram Equalization & DCP
├── fusion_based.ipynb         # Fusion-Based Method
├── retinex_method.ipynb       # Retinex Image Enhancement
├── images/                    # Input and Output Samples
└── README.md                  # Project Documentation
```

### 📂 Key Files

- **CLAHE.ipynb** – Implements CLAHE enhancement.
- **DCP.ipynb** – Implements Dark Channel Prior dehazing.
- **HE&DCP.ipynb** – Combines histogram equalization and DCP.
- **fusion_based.ipynb** – Executes fusion-based enhancement.
- **retinex_method.ipynb** – Applies the Retinex method.
- **images/** – Contains input and output samples for each method.

---

## ▶️ Usage Guide

1. **Clone the Repository**

```bash
  git clone https://github.com/Vikas5050/Underwater-Image-Processing.git
  cd Underwater-Image-Processing
```

2. **Set Up Environment**

Ensure Python is installed on your system. Recommended version: **Python 3.x**.

3. **Install Dependencies**

```bash
  pip install opencv-python numpy matplotlib
```

4. **Run the Notebooks**

Open Jupyter Notebook and execute the desired enhancement method:

```bash
  jupyter notebook CLAHE.ipynb
```

---

## 📊 Sample Outputs

### 🎨 CLAHE

![Image](https://github.com/user-attachments/assets/e48a1112-4579-4c59-9b40-9ca0d7f0d99e)

### 🌑 Dark Channel Prior

![Image](https://github.com/user-attachments/assets/0629a0b0-789b-4470-be3c-708e7a310f49)

### 🔥 Fusion-Based Enhancement

![Image](https://github.com/user-attachments/assets/cfa4204b-2)

### 💡 Retinex Method

![Image](https://github.com/user-attachments/assets/efcc20c1-22bf-49a4-ba04-42a9964bf16c)

---

## 📈 Evaluation Metrics

We assess image enhancement quality through:

- **PSNR (Peak Signal-to-Noise Ratio):** Measures noise reduction.
- **SSIM (Structural Similarity Index):** Evaluates image structure preservation.
- **Contrast Gain:** Measures improvement in visual contrast.

---

## 📌 Future Improvements

- ✅ Implement deep-learning-based enhancement.
- ✅ Add real-time video enhancement support.
- ✅ Optimize methods for faster processing.
- ✅ Include user-friendly GUI for easy interaction.

---

## 🤝 Contribution Guidelines

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

### 🧰 Requirements

Ensure your contributions maintain code clarity and efficiency. Follow PEP-8 standards.

---

## 🙌 Acknowledgments

Special thanks to our guides **Dr. Bambam** and **Dr. Ashish Kumar Bhandari** for their continuous support and mentorship throughout the project.

---

---

💡 *"Bringing clarity to the unseen world beneath the waves."*

