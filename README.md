# ⚽ DS340W – Final Project: Pass Probability Prediction

This GitHub repository is for academic purposes only. The materials uploaded here are part of a course project on Applied Data Science at **The Pennsylvania State University** (University Park, PA).

**Course**: DS 340W – Applied Data Science (Spring 2025)  
**Project Title**: *Pass Probability Prediction: A Data-Driven Approach to Soccer Analysis*  
**Author**: Haozhe Shan (Simon)

---

## 🧾 Repository Contents

This repository contains the complete implementation, visualizations, and supporting materials for the final project submission. All external datasets and code references are credited to their respective publishers.

---

## 📂 Datasets

This project uses **open event-level data from StatsBomb**, retrieved using the [`statsbombpy`](https://github.com/statsbomb/statsbombpy) Python API.

- **Main Match**: 2022 FIFA World Cup Final – Argentina vs France
- **Transfer Test Match**: 2022 FIFA World Cup – Argentina vs Saudi Arabia

> *Note: Due to licensing, raw data is accessed through the API and is not directly uploaded to this repository.*

---

## 💻 Code Files

- **`DS340W_Final_Code.ipynb`** – Final code file used for model training, evaluation, and visualizations. Modular, well-commented, and compatible with Colab.
  
  Includes:
  - Spatial feature engineering (pass origin/destination, angle, distance)
  - Pass success classification using XGBoost and Logistic Regression
  - Transferability testing on a second match
  - ROC curve visualization and metric comparison

- **`DS340W_Modified_Code.ipynb`** – Early version containing modular platform setup and passing network visualizations.

---

## 🧠 Project Objective

The goal of this project is to develop an interpretable machine learning model to predict **whether a pass will be successful** in professional soccer, using event-level features such as:

- Pass start and end coordinates  
- Distance and angle of the pass  
- Derived spatial zones and feature interactions  

This model is inspired by the parent paper **SoccerMap** [1], which uses deep learning on full-field tracking data. In contrast, our approach uses interpretable features from event data and XGBoost to achieve solid predictive performance.

---

## 📈 Key Results

| Metric        | World Cup Final (Train/Test) | Group Stage Transfer Test |
|---------------|------------------------------|----------------------------|
| Accuracy      | 0.835                        | 0.849                      |
| Precision     | 0.891                        | 0.882                      |
| Recall        | 0.913                        | 0.939                      |
| F1 Score      | 0.902                        | 0.910                      |

These results highlight the **strong generalization ability** of our pass success model, even across different teams and match contexts.

---

## 🧪 Techniques Used

- **Machine Learning Models**: XGBoost, Logistic Regression  
- **Evaluation**: Accuracy, Precision, Recall, F1 Score  
- **Visualization**: mplsoccer passing plots, heatmaps, ROC curves  
- **Tools**: Python, pandas, matplotlib, scikit-learn, statsbombpy

---

## 📄 Final Deliverables

| File | Description |
|------|-------------|
| `DS340W_Final_Code.ipynb` | Final modular code with models, visualizations, and reproducibility |
| `Final_Report.docx` | Full research paper in IEEE format |
| `Final_Presentation.pptx` | 10–15 minute PowerPoint presentation |
| `Kaltura Link` | Final recorded oral presentation (link unlisted) |

---

## 📚 References

[1] Fernández, J., & Bornn, L. (2020). SoccerMap: A Deep Learning Architecture for Visually Interpretable Analysis in Soccer. [arXiv link](https://arxiv.org/abs/2010.10202)

---

## 👨‍🎓 Author

**Haozhe Shan (Simon)**  
Senior, Applied Statistics  
The Pennsylvania State University  
📫 Contact: your_email@psu.edu

---

> *This repository showcases a simplified, interpretable, and transferable ML-based approach for spatial analysis in modern soccer analytics.*
