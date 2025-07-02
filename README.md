# 🧠 Image-based Transfer Learning Spike Classifier (ITSC)

This project explores a novel approach to **spike sorting** by transforming neural spike waveforms into grayscale images and applying **transfer learning** using deep convolutional neural networks. By leveraging pretrained models like EfficientNet-B3 with attention mechanisms, we aim to classify spikes from large-scale neural recordings with high accuracy and scalability.

---

## 📌 What is Spike Sorting?

**Spike sorting** is the process of identifying and classifying action potentials (or "spikes") recorded from neurons using extracellular electrodes. Since a single electrode can pick up signals from multiple nearby neurons, spike sorting algorithms analyze the shape and timing of these waveforms to assign each spike to its likely source neuron.

This is a critical step in neuroscience research, enabling scientists to:
- Decode neural activity at the single-neuron level
- Study brain function and behavior
- Build brain-computer interfaces and neuroprosthetics

Traditional spike sorting relies on manual feature extraction and clustering. This project proposes an **image-based deep learning alternative** that automates and enhances the process.

---

## 🚀 Project Overview

- Converts spike waveform data into grayscale images
- Applies transfer learning using EfficientNet-B3 + CBAM (Convolutional Block Attention Module)
- Trains and evaluates models on datasets with **1000** and **3544** spike classes
- Compares performance across architectures and class scales

---


Overall Workflow- 
![image](https://github.com/user-attachments/assets/5838c9d6-fe3d-4dfc-be89-29dfd9d4dbd5)


Proposed Architecture-
![image](https://github.com/user-attachments/assets/1e768675-86fd-4ee4-be49-d9674272a078)


---

## 🧠 Model Architecture

- **Backbone**: EfficientNet-B3
- **Attention Module**: CBAM
- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy, Precision, Recall, F1-score

---

EfficientNet-B3 with CBAM Architecture for Image-based Spike Sorting-
![image](https://github.com/user-attachments/assets/58553cd3-4c50-4e89-89b6-ce6788f3fc72)

## 📈 Results

- High classification accuracy on both 1000 and 3544 class datasets
- Performance metrics include:
  - Top-k Accuracy
  - Confusion Matrix
  - Precision-Recall and ROC Curves
  - Classification Summary CSV

---

Comaprsion with other Pretrained models- 
![image](https://github.com/user-attachments/assets/4b7da045-2b71-43f9-924c-8b42ea15d882)

![image](https://github.com/user-attachments/assets/5f84be6f-9069-46d4-948c-79e98e67ecb3)

![image](https://github.com/user-attachments/assets/2c005825-fe84-4216-99c9-52dce46a2948)


Results- 
![image](https://github.com/user-attachments/assets/fa3a3d41-e86a-4ad8-a798-6878dfbe2e42)

Top- k accuracy-
![image](https://github.com/user-attachments/assets/594ecb11-b047-401f-ae64-2e1b897b57f8)

Precision-Recall Curves-
![image](https://github.com/user-attachments/assets/dabf7a15-90f9-4eaf-8190-86ebcb56f5e7)

ROC Curve- 
![image](https://github.com/user-attachments/assets/8b3fbde3-cf04-4409-b9f2-74e2023a5fc9)

Top Most Confused Classes- 
![image](https://github.com/user-attachments/assets/e79d852c-f3ba-4984-88ba-17b0fd7230e8)

Classification Summary-
![image](https://github.com/user-attachments/assets/6853a3ae-da5e-431e-9f98-b40ab927106a)


Overall comparison between 1000 classes and 3544 classes- 
![image](https://github.com/user-attachments/assets/29384664-eaa8-45ea-9228-14da2e33e23b)

Final comparison of all the proposed models for Multi-class spike classification-
![image](https://github.com/user-attachments/assets/39518711-ee5f-4a3d-ab01-1ec1996922f2)

* requires more training time


📎 References
• 	Spike Sorting - Wikipedia
• 	EfficientNet: Rethinking Model Scaling
• 	CBAM: Convolutional Block Attention Module






