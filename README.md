# Bengali Document Layout Analysis Challenge - BaDLAD

Bengali is the **fifth most spoken native language worldwide**, making it a critical focus for advancing computational tools and datasets. As part of the **BUET CSE Fest 2023**, the Department of Computer Science and Engineering at BUET partnered with **Bengali.AI** to present **DL Sprint 2.0**, a deep learning competition centered on **Bengali Document Layout Analysis**.

This challenge introduces **BaDLAD**, the **first multi-domain, large Bengali Document Layout Analysis Dataset**, offering participants a unique opportunity to develop innovative solutions for layout analysis.

---

## Competition Overview

- **Dataset**: A subset of the **BaDLAD dataset**, contributed by Bengali.AI, was used for training and evaluation.  
  Detailed information about the dataset can be found in the referenced [paper](#).  
- **Open Participation**: The competition was open to everyone, not just undergraduates. Participants from any institution were encouraged to join.  
 

---

## Model Development

For this competition, I fine-tuned various models to tackle the Bengali document layout analysis problem effectively. Below are the key highlights:

### Models Used

1. **Fast R-CNN with Detectron2**  
   - Fine-tuned for layout analysis using a subset of BaDLAD.  
   - **Hyperparameter Tuning**:
     - **Learning Rate**: Experimented with values such as `0.001`, `0.005`, and `0.01` to find the best configuration.  
     - **Warm-Up Iterations**: Applied warm-up steps to stabilize initial training, typically set to `1000 iterations`.  
     - **Max Iterations**: Set to `12000 iterations` for full training cycles.  
   - **Data Augmentation**:
     - Applied techniques such as rotation, scaling, cropping, and flipping to improve generalization.

2. **Custom Augmentation Strategies**  
   - Implemented additional augmentation methods to enhance model robustness and handle diverse document layouts.  

---

## Results

- Fine-tuned **Fast R-CNN** achieved promising results on the BaDLAD dataset, demonstrating its potential for Bengali document layout analysis.  
- Data augmentation and hyperparameter tuning significantly improved model accuracy and robustness.

---

**Model link:** https://www.kaggle.com/datasets/samratabduljalil/bengali-document-layout-analysis-dl-sprint-2-0

