# Ds340W-Project-Codes
# Soccer Pass Success Prediction Platform (Inspired by SoccerMap)

## Description
This project is a modular platform for predicting the success of soccer passes using spatial features derived from event-level data. It is inspired by the parent paper *SoccerMap: A Deep Learning Architecture for Visually-Interpretable Analysis in Soccer*.

## Key Features
- Feature engineering: origin, destination, distance, angle
- Model: XGBoost classifier (interpretable and lightweight)
- Visualization: heatmaps to emulate SoccerMap's output style
- Modular code for future extensions

## Setup
```bash
pip install -r requirements.txt
python main.py
