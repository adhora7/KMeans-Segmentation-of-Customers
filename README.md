# KMeans Segmentation of Customers
# 🛍️ Customer Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)
![Status](https://img.shields.io/badge/Status-Complete-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

A Machine Learning project that segments mall customers into distinct groups based on their **Annual Income** and **Spending Score** using the K-Means Clustering algorithm.

---

## Problem Statement

A mall wants to understand its customers better. Instead of treating all customers the same, we use unsupervised machine learning to automatically discover groups of customers with similar behavior — so the business can target each group with the right strategy.

---

## 📊 Dataset

**Mall Customers Dataset** — a classic beginner dataset for clustering.

| Column | Description |
|---|---|
| CustomerID | Unique ID for each customer |
| Gender | Male / Female |
| Age | Age of the customer |
| Annual Income (k$) | Annual income in thousands of dollars |
| Spending Score (1-100) | Score assigned by the mall based on spending behavior |

- **Rows:** 200 customers
- **Source:** [Kaggle - Mall Customers Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

## 🔍 What I Did

1. **Loaded and explored** the dataset using Pandas
2. **Scaled the features** using StandardScaler so both features have equal weight
3. **Found the optimal number of clusters** using:
   - Elbow Method (WCSS plot)
   - Silhouette Score (objective validation)
4. **Trained K-Means** with `k=5` and `k-means++` initialization
5. **Visualized** the 5 customer segments on a scatter plot
6. **Profiled each cluster** to understand what type of customer belongs to each group

---

##  Results — 5 Customer Segments Found

| Cluster | Annual Income | Spending Score | Type |
|---|---|---|---|
| 1 | High | High |  VIP Customers |
| 2 | High | Low |  Careful Spenders |
| 3 | Low | High | Impulsive Buyers |
| 4 | Low | Low |  Budget Customers |
| 5 | Medium | Medium |  Average Customers |

---

##  Tech Stack

- **Python 3**
- **Pandas** — data loading and manipulation
- **NumPy** — numerical operations
- **Matplotlib** — data visualization
- **Scikit-learn** — StandardScaler, KMeans, silhouette_score

---

##  How to Run

**1. Clone the repository**
```bash
git clone https://github.com/adhora7/KMeans-Segmentation-of-Customers.git
cd Kmeans-Segmentation-of-Customers
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the notebook**

Open `Kmeans Segmentation of Customers.ipynb` in Jupyter or Google Colab and run all cells.



---

## 📂 Project Structure

```
customer-segmentation/
│
├── Kmeans_Segmentation_of_Customers.ipynb   # Main Colab/Jupyter notebook
├── Mall_Customers.csv            # Dataset
├── Requirements.txt              # Dependencies
├── LICENSE                       # MIT License
└── README.md                     # This file
```

---

## 💡 Key Learnings

- Feature scaling is not optional — without it, larger-scale features dominate distance calculations
- The Elbow Method is visual and subjective; Silhouette Score gives a more reliable, quantitative answer
- Unsupervised learning can generate real business value without any labeled data
- Visualizing results is just as important as building the model itself

---

## 🙋 Author

**Faria Anowara Adhora**
- LinkedIn: [linkedin.com/in/Faria Anowara Adhora](https://www.linkedin.com/in/faria-anowara-adhora?utm_source=share_via&utm_content=profile&utm_medium=member_android)
- GitHub: [github.com/adhora7](https://github.com/adhora7)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

