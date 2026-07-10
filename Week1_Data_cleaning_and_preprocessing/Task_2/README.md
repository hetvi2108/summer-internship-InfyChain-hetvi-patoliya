🌸 Iris Species Classification — Exploratory Data Analysis
A structured, visual EDA of the Fisher Iris dataset using Python Analysing 150 specimens across 3 species and 4 morphological features.

📋 Table of Contents
Project Overview
Dataset Description
Project Structure
Technologies Used
Installation & Setup
Notebook Walkthrough
Key Findings
Visualisations
Feature Priority for Modelling
Recommended Next Steps
Data Quality
Author
🔍 Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on the classic Fisher Iris dataset. The primary goal is to understand the structure, distribution, and separability of three iris species — Setosa, Versicolor, and Virginica — using four morphological measurements.

The analysis answers three core questions:

Which species are easy to separate and which are difficult?
Which features carry the most discriminative information?
What is the best strategy for building a classification model?
📂 Dataset Description
Property	Value
Source	sklearn.datasets.load_iris
Rows	150 (50 per species)
Columns	5 (4 features + 1 label)
Missing Values	None
Balance	Perfectly balanced — 50 samples each
Features
Column	Unit	Description
Sepal Length	cm	Length of the outer floral leaf
Sepal Width	cm	Width of the outer floral leaf
Petal Length	cm	Length of the inner floral petal
Petal Width	cm	Width of the inner floral petal
Species	—	Target label: setosa / versicolor / virginica
📁 Project Structure
iris-eda/
│
├── iris.ipynb        # Main analysis notebook (10 sections, 31 cells)
│
├── plot_01_avg_features.png   # Grouped bar chart — mean values per species
├── plot_02_histograms.png     # 2×2 histogram grid — feature distributions
├── plot_03_boxplots.png       # 2×2 box plots — spread by species
├── plot_04_heatmap.png        # Pearson correlation heatmap
├── plot_05_scatter_sepal_petal.png   # Scatter: Sepal Length vs Petal Length
├── plot_06_overlap.png        # Overlap zone highlighted scatter
├── plot_07_scatter_widths.png # Scatter: Sepal Width vs Petal Width
├── plot_08_pairplot.png       # All-feature pair plot
│
└── README.md                  # This file
🛠 Technologies Used
Library	Version	Purpose
Python	3.8+	Core language
pandas	≥1.3	Data loading and manipulation
numpy	≥1.21	Numerical operations
matplotlib	≥3.4	Static plotting engine
seaborn	≥0.11	Statistical visualisation
scikit-learn	≥0.24	Dataset loading
jupyter	≥1.0	Interactive notebook environment
💡 Key Findings
1. Species Separability Hierarchy
Setosa         ███████████████  100% separable  (zero overlap with others)
Virginica      ████████░░░░░░░   52% distinct    (48% overlaps with Versicolor)
Versicolor     ████░░░░░░░░░░░   12% distinct    (88% overlaps with Virginica)
Setosa is trivially separable using a single petal-length threshold (~2.0 cm).
Versicolor and Virginica share a significant feature space; 88% of Versicolor specimens fall within the Virginica region when plotted on sepal × petal length axes.
2. Feature Correlation Highlights
Pair	r	Meaning
Petal Length ↔ Petal Width	+0.96	Near-perfect — both carry similar information
Sepal Length ↔ Petal Length	+0.87	Strong positive
Sepal Length ↔ Petal Width	+0.82	Strong positive
Sepal Width ↔ Petal Length	−0.43	Moderate negative
Sepal Width ↔ Sepal Length	−0.12	Essentially independent
3. Bimodal Distribution (Petal Features)
Both petal measurements show a sharp gap between 2.0–3.0 cm — no iris specimen has a petal in this range. This structural gap makes Setosa linearly separable with 100% accuracy using only a threshold rule.

📊 Visualisations
All 8 plots are saved as high-resolution PNG files (150 dpi) in the project root.

File	Description
plot_01_avg_features.png	Mean sepal/petal dimensions per species
plot_02_histograms.png	Frequency distribution of each feature
plot_03_boxplots.png	Spread, median, and outliers by species
plot_04_heatmap.png	Correlation matrix with annotations
plot_05_scatter_sepal_petal.png	2-D class separation by length dimensions
plot_06_overlap.png	Overlap zone between Versicolor and Virginica
plot_07_scatter_widths.png	Class separation by width dimensions
plot_08_pairplot.png	Complete 4×4 feature combination grid
🏆 Feature Priority for Modelling
Priority	Feature	Reason
1st	Petal Length	Strongest bimodal separation; isolates Setosa perfectly
2nd	Petal Width	Highly correlated with petal length (r = 0.96); adds redundant but powerful signal
3rd	Sepal Length	Provides secondary stratification; weak for Versicolor/Virginica alone
4th	Sepal Width	Most independent feature (r < 0.45 with all others); least discriminative solo
✅ Data Quality
Criterion	Status	Detail
Completeness	✅ Excellent	No missing values in any column
Class Balance	✅ Excellent	Exactly 50 samples per species
Outliers	✅ Excellent	Fewer than 1% of records; negligible impact
Consistency	✅ Excellent	No anomalous values or unit mismatches
The dataset requires no preprocessing and is production-ready for classification experiments.

👤 Author
Synent Technologies Internship Program Analysis Date: May 2026 Language: Python 3 Environment: Jupyter Notebook

This project is part of an academic internship EDA assignment. The Iris dataset is a public-domain benchmark originally introduced by Ronald A. Fisher (1936).
Data visualization of the Iris dataset using Python to explore patterns and compare species through meaningful charts and plots. 🌸📊
