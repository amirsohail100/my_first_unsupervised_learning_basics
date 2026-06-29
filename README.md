# 🤖 Unsupervised Learning: Core Foundations & Mathematical Frameworks

Welcome to my core machine learning repository. This space documents my comprehensive transition from **Supervised Learning**—where algorithms rely heavily on labeled ground-truth datasets—into the sophisticated domain of **Unsupervised Learning**.

The primary technical objective here is to design, implement, and analyze systems that extract hidden structures, intrinsic patterns, and continuous statistical representations directly from raw, unannotated data.

---

## 🗺️ Learning Roadmap & Progression Matrix

This repository serves as a major mathematical and architectural bridge in my AI development workflow. The progression map below outlines the technical journey:

---

## 🛠️ Theoretical Frameworks & Implementations

This module focuses on discovering hidden patterns, structures, and anomalies without explicit labels. Each submodule in this folder focuses on a distinct mathematical paradigm:

### 1. Partitioning & Density-Based Clustering (Group Discovery)

- **K-Means Clustering:** Implemented utilizing the Voronoi iteration framework. Optimal cluster selection is determined through the calculation of Within-Cluster Sum of Squares (WCSS) via the **Elbow Method**, cross-verified with the **Silhouette Coefficient** to measure cluster separation.
- **DBSCAN (Density-Based Spatial Clustering):** Developed to handle arbitrary structural topologies and eliminate systemic noise. Configured utilizing core distance parameters (`eps`) and minimum density neighborhoods (`min_samples`).
- **Hierarchical Agglomerative Clustering:** Built using bottom-up linkage strategies (Ward's linkage, complete linkage) and evaluated through structural **Dendrogram** projections.

### 2. Dimensionality Reduction & Vector Space Transformation

- **Principal Component Analysis (PCA):** An orthogonal linear transformation that maps data to a new coordinate system such that the greatest variance comes to lie on the first coordinate. Achieved via Singular Value Decomposition (SVD) of the covariance matrix.
- **t-Distributed Stochastic Neighbor Embedding (t-SNE):** A non-linear, probabilistic technique specifically optimized for embedding high-dimensional manifolds into 2D or 3D spaces for visual diagnostics.

---

## 📊 Technical Comparison & Evaluation Metrics

| Algorithm Name | Mathematical Basis               | Primary Application Field            | Evaluation Metric          |
| :------------- | :------------------------------- | :----------------------------------- | :------------------------- |
| **K-Means**    | Euclidean Distance Minimization  | Customer Segmentation, Quantization  | Inertia & Silhouette Score |
| **DBSCAN**     | Density-Connected Neighborhoods  | Anomaly Detection, Spatial Analytics | Core-Border-Noise Mapping  |
| **PCA**        | Eigenvalue Decomposition         | Feature Reduction, Noise Filtering   | Explained Variance Ratio   |
| **t-SNE**      | Kullback-Leibler (KL) Divergence | High-Dimensional Visualization       | Perplexity Stability       |

---

## 🧮 Mathematical Reference

To evaluate the geometric cohesion of the clustering algorithms without explicit external labels, the **Silhouette Coefficient** $s(i)$ for a single point is computed as follows:

$$s(i) = \frac{b(i) - a(i)}{\max(a(i), b(i))}$$

_Where:_

- $a(i)$ represents the mean intra-cluster distance between point $i$ and all other points in the same cluster.
- $b(i)$ represents the mean nearest-cluster distance from point $i$ to the points in the closest neighboring cluster.

---

## 💻 Tech Stack & Production Environment

The codebases contained within this directory are written completely in Python and lean heavily on specialized scientific computation environments:

- **Language:** Python 3.10+
- **Core Libraries:** NumPy (Linear Algebra), Pandas (Data Manipulation)
- **ML Frameworks:** Scikit-Learn, SciPy
- **Visualization Engine:** Matplotlib, Seaborn

---

## 📈 Key Execution & Data Pipelines

1. **Data Preprocessing:** Automatic handling of missing values, followed by robust standard scaling to guarantee zero mean and unit variance across features.
2. **Dimensionality Extraction:** Applying PCA to compress features while retaining more than 90% of the total variance.
3. **Model Training & Inference:** Executing parallelized optimization loops for K-Means or DBSCAN parameters.
4. **Visualization Engine:** Generating clean plots showing clear cluster boundaries, outliers, and density layers.

---

💡 _This repository is continuously updated as I explore more advanced clustering techniques, deep clustering, and generative frameworks._

```bash
git clone [https://github.com/amirsohail100/my_first_unsupervised_learning_basics.git](https://github.com/amirsohail100/my_first_unsupervised_learning_basics.git)
cd my_first_unsupervised_learning_basics
```
