# Calculative Foundation – Linear Algebra

## 📌Project Overview

This project focuses on applying **Linear Algebra concepts** to analyze students' academic performance in different subjects using Python.

## Objective

The main objective is to understand how vectors, matrices, matrix operations, linear transformations, eigenvalues, eigenvectors, and Principal Component Analysis (PCA) can be used to analyze real-world data.

## 📂Dataset Information

`student_scores.xlsx` — small, hand-checkable, fully reproducible.
The dataset contains marks of 5 students across 3 subjects.

| Student | Math | Physics | Chemistry |
|---|---:|---:|---:|
| S1 | 85 | 78 | 92 |
| S2 | 70 | 88 | 65 |
| S3 | 95 | 91 | 88 |
| S4 | 60 | 55 | 72 |
| S5 | 78 | 82 | 70 |

- Total Students: 5
- Total Subjects: 3
- Matrix Shape: (5, 3)

## 🛠️Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Tasks & Implementation

### Part A: Vector & Matrix Fundamentals

1. Represented each student's subject scores as a vector.
2. Calculated L1 Norm and L2 Norm.
3. Calculated dot products and angles between student vectors.
4. Performed cross product operations using 3D vectors.
5. Calculated vector projection and perpendicular residual.

### Part B: Matrix Operations

1. Created a student-subject matrix.
2. Performed matrix addition.
3. Performed matrix multiplication.
4. Calculated matrix transpose.
5. Checked matrix inverse and determinant.
6. Calculated the inverse of the Gram matrix (MᵀM).

### Part C: Linear Transformations & Geometry

1. Explained lines, planes, and hyperplanes.
2. Created a plane using three student vectors.
3. Checked whether other student vectors lie on the same plane.
4. Explored dimensionality from 2D to 3D and higher dimensions.

### Part D: Eigenvalues & Decomposition

1. Calculated the covariance matrix.
2. Computed eigenvalues and eigenvectors.
3. Calculated explained variance ratio.
4. Applied Principal Component Analysis (PCA).
5. Generated PCA scores for all students.

## Key Results

| Concept | Value | Insight |
| --- | --- | --- |
| L2 norms | S3 = 158.3, S4 = 108.7 | S3 strongest, S4 weakest |
| Angle S1–S3 | 4.9° | S1, S3 have almost identical profiles |
| Angle S2–S4 | 26.2° | most different profile shapes |
| Cross product ‖v1×v2‖ | 3751.6 | parallelogram area |
| Projection of v2 on v1 | 86.3% along v1 | S2 shares S1's profile but is stronger in Physics |
| det(M) | undefined (5×3) | non-square |
| det of 3×3 submatrix | −26,445 | S1, S2, S3 linearly independent |
| Eigenvalues of Σ | 377.6, 141.3, 5.9 | PC1 explains 71.9%, PC1+PC2 = 98.8% |
| PC1 loading | [0.68, 0.61, 0.41] | "general ability" axis |
| PC2 loading | [−0.16, −0.67, 0.73] | "physics vs chemistry" axis |
| PCA scores | S3 = +23.1 (PC1), S4 = −31.2 (PC1) | rank by general ability |

## 📊Visualizations

The project includes the following charts:

1. L1 and L2 Norm Comparison
2. Cosine Similarity Heatmap
3. Vector Projection Geometry
4. 3D Cross Product Visualization
5. PCA Scree Plot
6. PCA Biplot
7. Covariance Matrix Heatmap

Each visualization includes an interpretation to explain the results.

## 📒Project Files

- `PR4.Calculative_Foundation.ipynb` – Python code, calculations, outputs, and visualizations.
- `README.md` – Project documentation and result summary.
- `student_scores.csv` — dataset
- `Theory_Notes.pdf` — Part A theory with definitions
- `README.md` — this file
- `images/` — all labelled charts


## 🎓Conclusion
The data live in ℝ³ but effectively in a **2D subspace**: the first two
principal components explain **98.8%** of variance. PC1 is a "general
ability" axis on which every subject loads positively; PC2 contrasts
Physics and Chemistry. Dimensionality reduction from 3→2 loses only
~1.1% of information, justifying 2D visualisation and compression.

## ⭐ If you find this project useful

Feel free to explore the dashboard and dataset.

**Made with Python 📊**

## 👩‍💻 Author

**Jiya Patel**