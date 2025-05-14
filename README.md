# Stellar Classification via Log Scaled HR-Diagram Analysis
Intro ML project exploring stellar data through log-scaled temperature and luminosity.

---

## Data Analyzed by  
**Aidan O'Halloran**  
[linkedin.com/in/aohallx](https://www.linkedin.com/in/aohallx/)
May 2026  

---

## Hypothesis
**Can logarithmic scales of temperature and luminosity be used to reproduce a Hertzsprung–Russell-type diagram with this dataset?**

---

## Dataset Overview

This is a 6-class star dataset used for classification with deep learning approaches, sourced from Kaggle. It contains:

- Absolute temperature (K)  
- Relative luminosity (L/Lo)  
- Radius (R/Ro)  
- Absolute magnitude (Mv)  
- Star color  
- Spectral class (O, B, A, F, G, K, M)  
- Star type (e.g., White Dwarf, Red Giant, Main Sequence)

### Missing data was originally calculated using astrophysical formulas:
- Stefan–Boltzmann Law (to estimate stellar luminosity)  
- Wien’s Displacement Law (for surface temperature via wavelength)  
- Parallax-derived radius estimation  

**Source:**  
[https://www.kaggle.com/datasets/deepu1109/star-dataset/data](https://www.kaggle.com/datasets/deepu1109/star-dataset/data)

---

## Machine Learning Approach

This project applies a regression-based approach to explore the relationship between stellar temperature and luminosity. By transforming both features using a logarithmic scale, the goal was to replicate the structure of a Hertzsprung–Russell diagram.

Through exploratory data analysis and plotting, the log-scaled values of temperature and luminosity revealed distinct stellar groupings — including main sequence stars, white dwarfs, and supergiants. Outliers were also identified using IQR-based filtering, highlighting stars with unusual physical properties. The final jointplot confirms that logarithmic transformations of these variables provide a strong visual and mathematical foundation for modeling stellar classification.

---

## Techniques Used

- Exploratory Data Analysis (EDA)
- Logarithmic feature scaling (base-10)
- Outlier detection using the IQR method
- Data visualization with Seaborn & Matplotlib
- Regression-style analysis of stellar structure

---

## Key Findings

- Log-log plots of temperature vs. luminosity clearly show distinct clusters of stellar types
- Outliers in luminosity and radius were effectively flagged and explored
- Log transformations reveal relationships consistent with real astrophysical theory

---

## Project Files

```bash
├── notebook.ipynb       # Full Jupyter Notebook with analysis and visuals
├── predictStarTypes.csv
├── hrdiagram.jpg
└── README.md

