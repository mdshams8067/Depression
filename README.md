# Seeing, Observing, and Hearing Depression: An AI-driven Tri-Modal Diagnostic Approach

## 📖 Project Overview

Clinical depression diagnosis often relies on subjective assessments, which can be inconsistent and slow. This project addresses the need for objective, scalable diagnostic tools by developing and validating a novel multimodal AI framework. By analyzing behavioral markers from three distinct data streams, our model provides a more holistic and accurate approach to identifying depression severity.

Our key contributions are:

1.  **A New Tri-Modal Dataset:** A gold-standard dataset of 103 participants, uniquely combining audio, facial video, and eye-tracking data with ground-truth PHQ-9 scores.

2.  **A Novel GCN Architecture:** A new Graph Convolutional Network (GCN) designed to effectively fuse the three modalities and learn the complex relationships between them.

3.  **The MFFBM Module:** A key innovation, the Multi-Frequency Filter-Bank Module (MFFBM), which allows our GCN to capture both shared patterns (low-frequency) and subtle, unique diagnostic clues (high-frequency) that other models miss.

## ✨ Key Results

Our model demonstrates state-of-the-art performance in classifying depression severity.

* **📈 Excellent Performance on the 3-Class Severity Task:** Our model achieved a strong balance of metrics crucial for clinical relevance:
    * **Accuracy:** 79%
    * **Recall (Sensitivity):** 79%
    * **Precision:** 81%
    * **F2-Score:** 79%

* **📊 Strong Performance on the Binary Task (Depressed/Not-Depressed):** The model showed excellent performance in identifying the presence of depression:
    * **Accuracy:** 90%
    * **Recall (Sensitivity):** 80%
    * **Precision:** 86%
    * **F2-Score:** 95%
      
   These high Recall and F2 scores highlight the model's effectiveness in correctly identifying patients with depression.

* **🏆 Outperformed >10 Baselines**, including traditional machine learning algorithms and other deep learning models.

## 🧠 Model Architecture

Our framework uses three parallel streams to extract features from each modality. These features are then fed into our novel Graph Convolutional Network (GCN), which is enhanced by the Multi-Frequency Filter-Bank Module (MFFBM), to produce a final classification.
