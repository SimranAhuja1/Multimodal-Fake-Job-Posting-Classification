# Multimodal Fake Job Posting Detection

## Overview

This project focuses on detecting fraudulent job postings using a multimodal deep learning approach. Instead of relying solely on textual features, we combine both textual and visual signals to improve classification performance.

The core idea is to explore how feature fusion techniques enhance fraud detection accuracy compared to unimodal baselines.

---

## Problem Statement

Online job platforms are increasingly vulnerable to fraudulent listings. Traditional text-based detection systems often fail to capture multimodal inconsistencies present in scam postings.

This project investigates whether integrating image-based features with textual representations improves detection performance.

---

## Approach

### Text Modality
- Preprocessed job descriptions
- Generated textual feature representations
- Trained baseline classification models

### Image Modality
- Extracted image embeddings using ResNet50
- Generated structured visual feature vectors

### Fusion Strategies
- Early Fusion
- Late Fusion
- Intermediate Fusion

Performance across fusion strategies was evaluated and compared.

---

## Model Architecture

- ResNet50 for visual feature extraction
- Deep neural network classifiers for final prediction
- Fusion layers for combining multimodal embeddings

---

## Explainability (XAI)

We incorporated explainability techniques to interpret model decisions and analyze feature importance across modalities.

XAI outputs are available in the `xai_outputs/` directory.

---

## Repository Structure

```
Checkpoint_1/          → Initial model experiments
Checkpoint_2/          → Improved ResNet-based model
Final_Checkpoint/      → Final fusion implementation
data/                  → Dataset samples
docs/                  → Final project report
fusion/                → Fusion model implementations
xai_outputs/           → Explainability results
XAI_Multimodal.ipynb   → Analysis notebook
requirements.txt       → Reproducibility 
```

---

## Tech Stack

- Python
- PyTorch
- ResNet50
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## How to Run

### 1. Clone Repository

```bash
git clone https://github.com/SimranAhuja1/Multimodal-Fake-Job-Posting-Classification.git
cd Multimodal-Fake-Job-Posting-Classification
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

If requirements.txt is not available, install manually:

```bash
pip install torch torchvision pandas numpy scikit-learn matplotlib
```

### 3. Run Model

Navigate to the desired checkpoint directory and execute the training script.

Example:

```bash
python fusion/train_fusion_model.py
```

(Adjust script names based on your implementation.)

---

## Results

The multimodal fusion approach demonstrated improved classification performance compared to unimodal baselines.

Evaluation metrics used:
- Accuracy
- Precision
- Recall
- F1-Score

Detailed experimental results are documented in the final report.

---

## Project Report

The complete project report with methodology, experiments, and analysis is available here:

📄 `docs/Final Project Report.pdf`

---

## My Contributions

- Implemented multimodal fusion strategies
- Integrated ResNet-based visual feature extraction
- Conducted performance evaluation and model comparison
- Worked on explainability analysis (XAI)
- Organized experiment checkpoints and final evaluation

---

## Future Work

- Incorporating transformer-based text encoders (e.g., BERT)
- Hyperparameter optimization
- Deployment as a REST API
- Real-time fraud detection pipeline
