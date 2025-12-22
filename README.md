# 🧠 Clustering Analysis of Commercial Data in a Gold Processing Plant

## 📌 Problem Description

Gold processing plants generate large volumes of commercial and operational data related to mineral characteristics such as gold grade, coarse gold content, moisture, tonnage, and metallurgical recovery. Additionally, business-related attributes (e.g., sector) influence how these materials are processed and commercialized.

In many real-world scenarios, this information is analyzed only through descriptive statistics, limiting the identification of underlying patterns and meaningful groupings. This project applies unsupervised learning techniques to discover hidden structures within the data and provide a more informative segmentation.

---

> ⚠️ **Disclaimer**  
> The dataset used in this project is **synthetically generated** and does **not** correspond to real operational or commercial data from any specific gold processing plant.  
>  
> While the structure and variable relationships were designed to resemble realistic industrial scenarios, all values were randomly generated with controlled variability. The purpose of this dataset is **strictly educational and demonstrative**, ensuring that no confidential, sensitive, or proprietary information is disclosed.

---

## 💡 Proposed Solution

The proposed solution applies **K-Means Clustering** using a combination of:

- Scaled numerical variables  
- Categorical variables encoded with *One-Hot Encoding*  
- **Principal Component Analysis (PCA)** for dimensionality reduction and visualization  

The objective is to identify an optimal number of clusters that maximizes separation while maintaining internal cohesion.

---

## 📊 Key Results

- Different values of *K* were evaluated using the **Silhouette Score**
- The optimal clustering solution was achieved with **K = 3**
- The first two PCA components explain approximately **43% of the total variance**
- The clusters represent differentiated profiles based on:
  - Wet metric tons
  - Gold grade (Au)
  - Coarse gold percentage
  - Metallurgical recovery
  - Moisture content
  - Sector of origin

*These clusters help characterize distinct commercial and operational behaviors.*

---

## ▶️ How to Run the Project (Google Colab)

1. Open the notebook in **Google Colab**
2. Upload the dataset to the Colab environment or mount Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')
```
3. Install required dependencies (if not already available): 
```
!pip install pandas numpy scikit-learn matplotlib seaborn
```
4. Run all notebook cells sequentially to reproduce the analysis

---

## 📁 Project Structure

```
├── data/
│   └── raw_data.csv
├── notebooks/
│   └── analysis.ipynb
├── results/
│   └── figures/
└── README.md
```

---

## 🛠️ Technologies Used

- Python 3  
- Google Colab  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  

---

## 🔬 Methodology

1. Exploratory Data Analysis (EDA) to understand data distributions, variable ranges, and initial patterns  
2. Data cleaning and wrangling, including the detection and correction of inconsistent or improperly recorded values (e.g., malformed dates and logical constraints)  
3. Feature selection based on domain knowledge and multicollinearity considerations  
4. Scaling of numerical variables to ensure comparable feature magnitudes  
5. Encoding of categorical variables using One-Hot Encoding  
6. Application of K-Means clustering for multiple values of *K*  
7. Model evaluation using the Silhouette Score  
8. Dimensionality reduction with PCA for visualization and interpretability  
9. Interpretation and analysis of the resulting clusters  

---

## 📚 Conclusions and Learnings

- Unsupervised learning techniques are effective for identifying hidden patterns in commercial datasets
- The inclusion of categorical variables can significantly influence clustering outcomes
- PCA improves interpretability when working with high-dimensional data
- Data preprocessing decisions strongly affect clustering performance

*This project demonstrates practical skills in data cleaning, unsupervised machine learning, and analytical reasoning using real-world-inspired data.*

---

## 📬 Contact

- Name: Jhoel Palomino
- LinkedIn: www.linkedin.com/in/jhoelpe
- Email: jhoel.pe@outlook.com
- GitHub: https://github.com/JhoelPalomino