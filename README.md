Fruit-Quality-Classification-Benchmark
A comparative study of MobileNet and EfficientNet for classifying fruit quality (Apples, Bananas, Oranges, Pomegranates) into Good, Bad, and Mixed categories.

Fruit Quality Classification Benchmark

📌 Project Overview
This project focuses on the automated classification of fruit quality using Deep Learning techniques. The goal is to categorize images of fruits into three distinct classes— Good, **Bad**, and **Mixed**—to assist in agricultural quality control and freshness detection.

The project evaluates and compares the performance of two popular Convolutional Neural Network (CNN) architectures:
1.  **MobileNet** (Lightweight, optimized for mobile devices)
2.  **EfficientNet** (Designed for high accuracy and efficiency)

## 📂 Dataset
The dataset comprises images of four different fruit types tracked over time to simulate aging and decay:
* 🍎 **Apple**
* 🍌 **Banana**
* 🍊 **Orange**
* 🧶 **Pomegranate**

Each fruit category is split into three labels based on visual quality:
* **Good:** Fresh, high-quality fruit.
* **Bad:** Rotten or visibly decayed fruit.
* **Mixed:** Fruits showing early signs of degradation or partial decay.

## 📊 Model Performance & Results
We trained both models on the dataset and evaluated them based on **Accuracy**, **Precision**, **Recall**, and **F1-Score**. Below is a summary of the validation accuracy for each fruit type based on the training reports.

| Fruit Type | MobileNet Accuracy | EfficientNet Accuracy | Key Observation |
| :--- | :--- | :--- | :--- |
| **Apple** | ~67% | **100%** | EfficientNet significantly outperformed MobileNet, which struggled to distinguish 'Mixed' quality apples. |
| **Banana** | ~98.8% | **99.6%** | Both models performed exceptionally well, with EfficientNet having a slight edge. |
| **Orange** | ~46% | **100%** | MobileNet failed to converge effectively for Oranges, whereas EfficientNet achieved perfect classification. |
| **Pomegranate** | ~98.5% | **99.6%** | Both models achieved high accuracy, proving the dataset features were distinct for both architectures. |

### 📈 Visualizations
Detailed performance metrics, including **Confusion Matrices** and **Training/Validation Accuracy Plots**, can be found in the attached reports:
* [`Apple.pdf`](./Apple.pdf)
* [`Banana.pdf`](./Banana.pdf)
* [`Orange.pdf`](./Orange.pdf)
* [`Pomegranate.pdf`](./Pomegranate.pdf)

## 🧠 Methodology
1.  **Data Preprocessing:** Images were resized and normalized. Data augmentation techniques were likely applied to improve generalization.
2.  **Model Training:**
    * Models were trained over multiple epochs.
    * **Loss Function:** Categorical Cross-Entropy.
    * **Optimizer:** Adam/SGD (inferred).
3.  **Evaluation:** Models were tested on a validation set to generate confusion matrices and classification reports.

## 🚀 Future Scope
* **Hyperparameter Tuning:** Improve MobileNet performance on Apples and Oranges.
* **Real-time Detection:** Deploy the EfficientNet model using a web interface (e.g., Streamlit or Flask).
* **Expanded Dataset:** Incorporate more fruit varieties (e.g., Strawberry, Guava).

## 👤 Author
[Your Name/Username]
