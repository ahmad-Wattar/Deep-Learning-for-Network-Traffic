# Deep Learning Network Traffic Classification

##  Project Overview

This project was developed as part of a **master’s degree program at Martin Luther University Halle-Wittenberg (Germany)** within the course **Machine Learning and IT Security**.

The goal of this work is to analyze and classify network traffic using a combination of:

- Unsupervised Learning (Clustering)
- Deep Learning (Neural Networks)

The project focuses on identifying patterns in network flow data and building a supervised classification model based on automatically generated labels.

---

##  Objective

The main objective is to classify different types of network traffic (e.g., TCP, UDP, DNS-based communication) using machine learning techniques.

The workflow is divided into two main parts:

### 1. Unsupervised Learning
- Exploration of network flow data
- Feature engineering and preprocessing
- Clustering using algorithms such as:
  - K-Means
  - DBSCAN
- Analysis and interpretation of clusters
- Manual labeling of clusters (e.g., HTTP, DNS, background traffic)

### 2. Deep Learning
- Creation of a labeled dataset based on clustering results
- Training of a neural network classifier using TensorFlow / Keras
- Evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1-score

---

## 📊 Dataset

The dataset used in this project is based on network flow measurements extracted from Wireshark captures.

- Input file: `aneaf.xlsx`
- Contains network flow features such as:
  - Source / Destination IP
  - Source / Destination ports
  - Protocol type
  - Duration
  - Packet statistics (bytes, packets, rates, etc.)
  - Timing features (IAT, packet intervals)

---

##  Feature Engineering

Several additional features were engineered to improve model performance:

- Payload ratio
- Average packet size
- Byte rate
- Packet rate
- Average time per packet

These features help better distinguish between different traffic behaviors.

---

##  Project Structure

```text
Deep-Learning-Network-Traffic-Classification/
│
├── aneaf.ipynb              # Main Jupyter Notebook (solution)
├── aneaf.xlsx               # Raw dataset
├── aneaf.csv                # Converted dataset (generated during execution)
├── Aufgabenstellung.pdf     # Assignment description
├── README.md                # Project documentation


## Technologies Used

- Python 3  
- Pandas  
- NumPy  
- Scikit-learn (KMeans, DBSCAN, preprocessing, metrics)  
- TensorFlow / Keras (Deep Learning model)  
- Matplotlib / Seaborn (visualization)  
- Jupyter Notebook  

---

## Workflow Summary

- Load and preprocess network flow data  
- Perform exploratory data analysis (EDA)  
- Engineer meaningful features  
- Apply clustering algorithms (unsupervised learning)  
- Interpret clusters and assign labels  
- Train a deep learning classifier  
- Evaluate model performance  

---

##  Results

The project demonstrates that:

- Network traffic contains meaningful statistical patterns  
- Clustering can separate traffic types without labels  
- Neural networks can learn from pseudo-labels  
- Feature engineering significantly improves classification performance  

---

##  Academic Context

This project was created as part of a Master’s program at:

**Martin Luther University Halle-Wittenberg (MLU Halle)**  
Course: Machine Learning and IT Security  
Semester: Winter Term 2025/26  

The full assignment description is included in:  
`Aufgabenstellung.pdf`

---

## Notes

- The project is fully reproducible from the notebook  
- All steps (EDA → clustering → deep learning) are documented  
- Intended for academic and learning purposes  
