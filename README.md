# 🧠 Enhancing Low-Resolution Facial Emotion Recognition via Super-Resolution

This project investigates the use of **Super-Resolution (SR)** techniques to improve the accuracy of **Facial Emotion Recognition (FER)** systems on low-resolution images.\
We explore how GAN-based restoration—specifically **GFPGAN**—can enhance degraded facial images before they are passed to deep learning classifiers.

---

## 🌟 Project Objective

While most state-of-the-art FER models are trained on high-resolution datasets, real-world scenarios (e.g. surveillance cameras, video calls) often involve low-resolution images.\
This project proposes a deep learning pipeline that uses **GFPGAN for facial enhancement**, followed by classification with **pre-trained CNN models (e.g. VGG-16)** fine-tuned for emotion recognition.

---

## 🧪 Research Question & Hypothesis

> **Question**: Can Super-Resolution techniques improve the accuracy of emotion recognition from low-resolution images?

> **Hypothesis**: Applying Super-Resolution as a preprocessing step will significantly enhance classification performance compared to training directly on low-resolution images.

---

## 🔍 Key Components

- 🧬 **GFPGAN** – A GAN-based facial restoration framework using pretrained StyleGAN priors and U-Net architecture with CS-SFT layers.
- 📆 **KDEF Dataset** – 4,900 high-quality facial images across 7 emotional states, used as the benchmark dataset.
- 🤠 **Deep CNNs** – Pre-trained models (e.g., VGG-16, VGG-19) used for emotion classification.
- 📉 **Baseline vs. Enhanced Comparison** – Experiments are conducted in two phases:
  1. Train/test model directly on low-resolution data
  2. Train/test model on enhanced low-res data using GFPGAN

---

## 🏗️ System Architecture

```
KDEF High-Res Image
     │
[ Downsample to Low-Res ]
     │
Low-Res Image
     │
[ GFPGAN Enhancement ]
     │
[ Pre-Trained CNN Classifier ]
     │
Emotion Prediction
```

---

## 📊 Expected Impact

Improving FER for low-resolution images expands its application in:

- 👮 Security & surveillance systems
- 💬 Human-computer interaction (HCI)
- 🧑‍⚕️ Remote patient monitoring and mental health analysis

---

## 📚 Related Work

This project builds on:

- [Akhand et al. 2021](https://arxiv.org/abs/2101.04061) – Transfer learning with VGG models for FER
  [GitHub Repo](https://github.com/ShuvenduRoy/FER_TL_PipelineTraining)
  
- [Wang et al. 2021](https://www.mdpi.com/2079-9292/10/9/1036) – GFPGAN for real-world blind face restoration
  [GFPGAN GitHub Repo](https://github.com/TencentARC/GFPGAN)

---

## 🧑‍💼 Authors

- **Tzuf Lahan** ([lahantz@post.bgu.ac.il](mailto\:lahantz@post.bgu.ac.il) Or [zupl1234@gmail.com](mailto\:zupl1234@gmail.com))\
  M.Sc. student in Information Systems and Software Engineering, specializing in Deep Learning and Medical Imaging

- **Noa Stern** ([noaster@post.bgu.ac.il](mailto\:noaster@post.bgu.ac.il))\
  M.Sc. student in Information Systems and Software Engineering, with a research focus on the relationship between anxiety and temporal patterning.

---

## 📌 License

This project is for academic research purposes only.

