# 🧬 Colorectal Cancer Detection & Stage Prediction Using Deep Learning

An AI-powered tool that classifies colorectal cancer stages from histopathological images using deep learning. Built with a custom CNN model and GUI using Tkinter, the system identifies whether the tissue sample is cancerous and if so, predicts the cancer stage (1 to 4) with explanations.

![GUI Preview](screenshots/gui_preview.png)

---

## 📁 Dataset

**LC25000 Dataset**  
- Contains histopathological images of colon tissues.
- Used folders: `colon_n` (Normal), `colon_aca` (Malignant - Adenocarcinoma).
- `colon_aca` folder clustered using **KMeans** into 4 stages for staging purposes.

> 📌 Dataset source: [LC25000 Dataset](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images)

---

## 🧠 Models Used

| Model Name | Architecture | Accuracy | Notes |
|------------|--------------|----------|-------|
| `colorectal_staging_model.h5` | Custom CNN | ✅ Trained | Used in final GUI |
| `colon.h5` | VGG16 (Transfer Learning) | ✅ Trained | Optional |
| `colon_resnet.h5` | ResNet50 (Transfer Learning) | ✅ Trained | Optional |

---

## 💻 Features

- 🔍 Predicts **presence of cancer**
- 📊 Classifies into **Stage 1 to Stage 4** if cancer is present
- 🖼️ Displays the selected image
- 📖 Provides **stage-wise explanations**
- 🎨 **Stylish GUI** built using `Tkinter`
- 📈 Accuracy graph plotted after training
- 📂 Images organized into stage folders using **KMeans**

---

## 🎨 GUI Preview

<img src="screenshots/gui_full.png" width="500">

---

## 📈 Sample Graphs

| Accuracy | Loss |
|---------|------|
| ![Acc](screenshots/acc.png) | ![Loss](screenshots/loss.png) |

---

## 🚀 Installation & Running

1. **Clone the repository**  
```bash
git clone https://github.com/yourusername/colorectal-cancer-stage-detector.git
cd colorectal-cancer-stage-detector
