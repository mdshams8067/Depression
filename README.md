# Seeing, Observing, and Hearing Depression: An AI-driven Tri-Modal Diagnostic Approach

## Project Overview

Clinical depression diganosis heavily relies on self reported assessments that are subjected to bias. Our project works to eliminate this subjective bias by developing and validation a novel multimodal AI framwork that will be a more objective diagnositc tool. We use three distinct modalities to track the behavioural cues that depression persons show to give a more accurate approach to identifyting depression severity.

Our key contributions are:

1.  **A New Tri-Modal Dataset:** A gold-standard dataset of 103 participants. This dataset includes audio, facial video, and saliency data with ground-truth PHQ-9 scores.

2.  **High Frequency Signals:** Exisitng graph based depression detection methods primarily focus on low frequency signals. We demonstrate the high frequency signals contain critical information for depression detection

3.  **Advanced Graph filtering:** The Multi-Frequency Filter-Bank Module (MFFBM), which allows our GCN to capture both shared patterns (low-frequency) and subtle, unique diagnostic clues (high-frequency) that other models miss.

4.  **Saliency map fusion:** Use of saliency map in a multimodal approach has not been explored before us.

## ✨ Key Results

The evaluation was done in two tasks - 
1. 3 Class severity classification
   a. No Depression
   b. Mild to Moderate Depression
   c. Severe Depression
3. Binary (Depressed/Not-Depressed) classification

* **📈 3-Class Severity Task:** Our model demonstrated strong performance in metrics crucial for clinical relevance.
    * **Sensitivity:** 79%
    * **Specificity:** 87%
    * **F2-Score:** 79%

* **📊 Binary Task (Depressed/Not-Depressed):** Our model showed execellent performance in identyfing depressed patients highlighted by the high Sensitivity score
    * **Sensitivity:** 98%
    * **Specificity:** 80%
    * **F2-Score:** 95%
      
   These high Recall and F2 scores highlight the model's effectiveness in correctly identifying patients with depression.

* **🏆 Outperformed >10 Baselines**, including traditional machine learning algorithms and other deep learning models.

## 🧠 Model Architecture

Our framework first extracts features from each modality in three separate streams. These features are then passed through our Graph Convolution Network(GCN) and the Multi-Frequency Filter Bank Module(MFFBM) that uses both high and low pass signals to do the final classification
