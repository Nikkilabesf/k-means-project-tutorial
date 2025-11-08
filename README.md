<!-- ✨ PRETTY TECH GIRL - OFFICIAL README TEMPLATE ✨ -->

<div align="center">

# 🏡✨ **HOUSE GROUPING SYSTEM** ✨  
### *K-Means + Supervised Learning Project by Pretty Tech Girl 💖*

---

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/scikit--learn-Machine%20Learning-orange?logo=scikitlearn&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-Data%20Viz-lightblue?logo=plotly&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/License-MIT-purple">
  <img src="https://img.shields.io/badge/Made%20with-%F0%9F%92%96%20by%20Pretty%20Tech%20Girl-pink">
</p>

---

</div>

<div align="center">

> 💬 “Sourced from Earth, Prepared for Code.”  
> — *Pretty Tech Girl 🪄*

</div>

---

## 🌍 **Project Overview**
This project groups California housing data into **regions** based on **median income** and **geographic coordinates** using **Unsupervised Learning (K-Means)** — then trains a **Supervised Model (Random Forest)** to predict which region a new house belongs to.

📊 **Dataset:** California Housing Census (1990)  
Includes the following features:  
- 🧭 `Latitude`  
- 📍 `Longitude`  
- 💰 `MedInc` *(Median Income)*  

---

## ⚙️ **Tech Stack**

| 🧠 Tool | 💡 Purpose |
|----------|-------------|
| 🐍 **Python 3.12** | Core programming |
| 📘 **Pandas / NumPy** | Data cleaning & analysis |
| 🧮 **Scikit-learn** | Machine Learning (K-Means, Random Forest) |
| 📊 **Matplotlib / Seaborn** | Data Visualization |
| 💾 **Joblib** | Save & load trained models |

---

## 🧪 **Workflow Summary**

1. **Data Preparation**  
   - Load dataset & extract relevant columns (`Latitude`, `Longitude`, `MedInc`).  
   - Split into `train` and `test` sets.

2. **Unsupervised Clustering (K-Means)**  
   - Build a K-Means model with 6 clusters.  
   - Add a new column `cluster` representing region assignment.  
   - Visualize clusters across California.

3. **Prediction with Test Set**  
   - Use trained K-Means model to predict new house clusters.  
   - Validate cluster consistency visually.

4. **Supervised Classification (Random Forest)**  
   - Use K-Means clusters as labels.  
   - Train Random Forest classifier.  
   - Evaluate using accuracy, precision, and recall metrics.

5. **Model Saving**  
   - Save both models in a `/models` folder using Joblib.  

---

## 📈 **Visualization Example**
<img width="695" height="547" alt="524442f4-cbf6-49fe-9124-beacc17dcbf5" src="https://github.com/user-attachments/assets/fd2ae5a2-9e2d-4caa-9d22-bcd9bc77f5fb" />
<img width="695" height="547" alt="1b62f7c2-d5b5-4a28-972d-9830438c5d01" src="https://github.com/user-attachments/assets/37f31f8b-832f-4e85-aee4-8a406454b98c" />
<img width="600" height="435" alt="da49d7b6-f290-4993-87a4-49141e57b68d" src="https://github.com/user-attachments/assets/663fa344-f1d7-46f6-aefa-0195fefd8501" />
🖼️ Each color represents a unique regional grouping by median income.


🧠 Results Summary

✨ Highlights:

✅ 6 clusters form clear geographic and economic boundaries.

💰 Higher-income clusters concentrate along the coast.

🌄 Inland regions show lower-income clusters.

🎯 Random Forest Accuracy: ~85–90%.

🌟 Most Influential Feature: MedInc.




🧰 Repository Structure
📦 house-grouping-system
│
├── data/
│   └── housing.csv
│
├── models/
│   ├── kmeans_model.pkl
│   └── random_forest_model.pkl
│
├── notebooks/
│   └── housing_clustering.ipynb
│
├── README.md
└── .gitignore





💡 Future Improvements

🌀 Add DBSCAN or Agglomerative Clustering for comparison.

🗺️ Use Folium or Plotly Mapbox for geospatial heatmaps.

🧱 Build a Streamlit or Gradio dashboard to visualize clusters.

⚡ Create a FastAPI endpoint to serve model predictions.






<div align="center">
👩🏽‍💻 Author
✨ Tenika Powell

Machine Learning Engineer | Healthcare AI | Pretty Tech Girl Founder

💖 Passionate about turning real-world data into intelligent, human-centered technology.
Currently focused on ML & Deep Learning applications in healthcare and creative AI innovation.

📍 Michigan, USA

🔗 Connect With Me
💼 LinkedIn
 | 💻 GitHub
 | 📧 powell.tenika.n@gmail.com

✨ Sourced from Earth, Prepared for Code.

</div> ```

