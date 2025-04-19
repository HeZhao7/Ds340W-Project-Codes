# ⚽ DS340W – Final Project: Pass Probability Prediction

This GitHub repository is for academic purposes only. The materials uploaded here are part of a course project on Applied Data Science at **The Pennsylvania State University** (University Park, PA).

**Course**: DS 340W – Applied Data Science (Spring 2025)  
**Project Title**: *Pass Probability Prediction: A Data-Driven Approach to Soccer Analysis*  

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

## 📚 References

[1] Fernández, J., & Bornn, L. (2020). SoccerMap: A Deep Learning Architecture for Visually Interpretable Analysis in Soccer. [arXiv link](https://arxiv.org/abs/2010.10202)

---
