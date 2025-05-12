# 🧠 Federated Learning for Eye Disease Prediction

A secure, privacy-preserving medical AI framework designed to detect ocular diseases like **glaucoma**, **diabetic retinopathy**, and **macular degeneration** using **federated learning (FL)** and **Convolutional Neural Networks (CNNs)**. The system integrates **Elliptic Curve Cryptography (ECC)** to ensure encrypted model transmission across decentralized nodes.

## 📌 Project Overview

- **Goal**: Early prediction of eye diseases while preserving patient data privacy.
- **Technique**: Federated Learning using CNN (VGG16/ResNet50) trained on local devices without sharing raw data.
- **Security**: ECC for encrypted model updates.
- **Dataset**: Fundus images from Kaggle (e.g., APTOS, Indian Diabetic Retinopathy).

## ⚙️ Features

- Decentralized model training with **TensorFlow Federated** / **PySyft**.
- Secure model sharing using **ECC encryption**.
- Model evaluation using metrics like **accuracy**, **precision**, **F1-score**, and **AUC**.
- Support for **query-based prediction** and **automated appointment booking**.
- Cloud-compatible (GCP, AWS, Azure).

## 🧱 Modules

1. **Dataset Collection**: Aggregates anonymized eye scan images.
2. **Model Building**: CNN-based model training with federated averaging.
3. **Model Encryption**: Encrypts models using ECC before transmission.
4. **Query Processing**: Routes user queries to local inference models.
5. **Model Decryption**: Validates and decrypts model at the user end.
6. **Prediction Engine**: Returns disease labels with confidence scores.
7. **Appointment System**: Schedules follow-ups based on results.

## 🧪 Tech Stack

- **Language**: Python
- **Frameworks**: PyTorch, TensorFlow Federated, Flower, PySyft
- **Libraries**: OpenCV, Albumentations, Torchvision, NumPy
- **Cloud**: GCP / AWS EC2 & S3 / Firebase
- **Security**: ECC, SMPC, Differential Privacy
- **Visualization**: Weights & Biases (wandb)

## 📊 Results

| Model            | Accuracy | AUC    | F1-Score |
|------------------|----------|--------|----------|
| ResNet (partial) | 95.73%   | 96.45% | 94.98%   |
| VGG16 (full)     | 87%      | 87.41% | 86.32%   |

## 🖼️ Screenshots

- Home Dashboard
- Doctor Registration & Login
- Diagnosis Summary
- Heatmaps from Grad-CAM (Explainability)

## 🔐 Security

- **Encryption**: Elliptic Curve Cryptography (ECC)
- **Threat Mitigation**: Gradient leakage, model poisoning, eavesdropping
- **Secure Environments**: TPM, HSM, Intel SGX support

## 🚀 Setup Instructions

1. Clone this repository.
2. Install requirements using `pip install -r requirements.txt`.
3. Run `main.py` to start training/inference.
4. Optional: Launch `appointment_module.py` for booking interface.

## 📄 Report

Full documentation and source code included in [`batch 7 report.pdf`](./batch%207%20report.pdf)

## 👥 Authors

- Kanniga Saraswathy M
- Madhumitha P
- Monish Vidyarthi R
- Subalatha A

## 🎯 Future Enhancements

- Blockchain-based audit trails
- Reversible watermarking for image authentication
- Integration with national health record systems

---

🏥 *Final Year Project — B.Tech in Artificial Intelligence and Data Science, K. Ramakrishnan College of Technology, May 2025*
