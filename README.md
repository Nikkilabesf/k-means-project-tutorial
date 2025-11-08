# 🏡 House Grouping System — K-Means + Supervised Learning  
*By Pretty Tech Girl ✨*  

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/scikit--learn-ML-orange?logo=scikitlearn&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-Data%20Viz-lightblue?logo=plotly&logoColor=white">
  <img src="https://img.shields.io/badge/License-MIT-green">
  <img src="https://img.shields.io/badge/Made%20with-%F0%9F%92%96%20by%20Pretty%20Tech%20Girl-pink">
</p>

---

## 🌍 Project Overview  
This project groups California housing data into regions based on **median income and geographic coordinates** using **unsupervised learning (K-Means)** — then trains a **supervised model (Random Forest)** to predict the cluster (region) a new house belongs to.

📊 The dataset is sourced from the **1990 California Census** and contains:  
- 🧭 **Latitude**  
- 📍 **Longitude**  
- 💰 **Median Income (MedInc)**  

---

## ⚙️ Tech Stack
| Tool | Purpose |
|------|----------|
| 🐍 Python 3.12 | Core programming |
| 🧠 Scikit-learn | ML algorithms (K-Means, Random Forest) |
| 📊 Matplotlib | Visualization |
| 🧾 Pandas / NumPy | Data wrangling |
| 💾 Joblib | Model saving/loading |

---

## 🧪 Workflow Summary
1. **Load & Clean Data**  
   Load housing dataset and extract relevant columns (Latitude, Longitude, MedInc).  

2. **Unsupervised Clustering (K-Means)**  
   - Create 6 clusters (`n_clusters=6`).  
   - Add `cluster` labels to the dataset.  
   - Plot clusters geographically to observe region separation.  

3. **Prediction on Test Set**  
   - Apply K-Means model to unseen test data.  
   - Overlay both sets to confirm consistency.  

4. **Supervised Classification (Random Forest)**  
   - Use cluster labels as training targets.  
   - Train a classifier to predict cluster IDs.  
   - Evaluate accuracy and feature importance.  

5. **Save Models**  
   Store both trained models for future predictions using Joblib.

---

## 📈 Visualization Example
```python
plt.scatter(df["Longitude"], df["Latitude"],
            c=df["cluster"], cmap="viridis", s=15)
plt.title("California Housing Clusters by Region")
plt.xlabel("Longitude")
plt.ylabel("Latitude")
%matplotlib inline
plt.show()


🧠 Results Summary

✅ 6 clusters form clear patterns across California.

💰 Higher-income areas cluster distinctly along the coast.

🌄 Inland, lower-income regions form separate groups.

🔮 Random Forest accuracy: ~85–90%, showing strong model reliability.

⭐ Top feature: MedInc (median income strongly drives cluster boundaries).

REPOSITORY STRUCTURE
.
├── data/
│   └── housing.csv
├── models/
│   ├── kmeans_model.pkl
│   └── random_forest_model.pkl
├── notebooks/
│   └── housing_clustering.ipynb
├── README.md
└── .gitignore





# Clone repository
git clone https://github.com/Nikkilabesf/house-grouping-system.git
cd house-grouping-system

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook notebooks/housing_clustering.ipynb



👩🏽‍💻 Author

👋 Hi, I’m Tenika Powell — a Machine Learning Engineer passionate about Healthcare AI, data-driven solutions, and creative tech innovation.

🌐 Brand: Pretty Tech Girl 💖
💼 Machine Learning Engineer | Data Science | Healthcare AI | FastAPI | TensorFlow | Python
📍 Based in Michigan, USA

📫 Connect with me:

🔗 https://github.com/Nikkilabesf

💼 LinkedIn: https://www.linkedin.com/in/tenika-powell-ba35022b0/

📧 powell.tenika.n@gmail.com
