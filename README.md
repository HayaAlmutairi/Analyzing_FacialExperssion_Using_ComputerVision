# Implicit Tourist Experience Evaluation Using Deep Learning

This project implements an **implicit rating system** using facial expression recognition to evaluate client emotions and tourist experiences. By leveraging deep learning, the system provides a scalable and automated alternative to traditional feedback methods like surveys.

## Overview
Traditional methods for gathering feedback (surveys, comment sections) are often inaccurate and have limited reach. This system addresses these issues by fine-tuning a deep learning model on the **AffectNet dataset** using a **hierarchical classification** method.

### Key Features
* **Hierarchical Classification:** Uses ResNet-50 models to first categorize emotions into Positive and Negative groups, followed by specific subcategories (Happy, Surprise, Sad, Fear).
* **Deep Learning Backbone:** Built on a fully fine-tuned **ResNet-50** architecture.
* **Gradio-Based Interface:** A user-friendly UI for testing and demonstration.
* **Ethical & Privacy Focused:** Includes features like optional image pixelation and bounding box annotations to ensure user privacy.

## Performance
The system demonstrates robust performance across the classification hierarchy:

| Classifier | Accuracy | F1-Score | Highlights |
| :--- | :--- | :--- | :--- |
| **Parent Classifier** | 84% | 81% | Balanced precision and recall. |
| **Positive Classifier** | 75% | 81% | Strongest performance in "Happy" detection. |
| **Negative Classifier** | 65% | 75% | High F1-score for "Fear" classification. |

## Technical Stack
* **Language:** Python
* **Libraries:** TensorFlow/Keras, OpenCV, Gradio, NumPy, Matplotlib
* **Dataset:** AffectNet (Hierarchical subset)
* **Architecture:** Fine-tuned ResNet-50

## 📁 Repository Structure
* `Code.ipynb`: Complete Jupyter Notebook containing data preprocessing, model training, evaluation, and the Gradio deployment.
* `README.md`: Project documentation.
