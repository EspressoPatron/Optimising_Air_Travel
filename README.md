# ✈️ Optimising Air Travel – Flight Delay Analysis & Prediction

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![SHAP](https://img.shields.io/badge/Explainable%20AI-SHAP-blueviolet)](https://shap.readthedocs.io/)
[![Project Status](https://img.shields.io/badge/Status-Completed-brightgreen)]()

---

## Overview

Flight delays are more than a nuisance — they disrupt passenger plans, increase airline costs, and create network-wide inefficiencies. This project leverages historical data and machine learning to predict both the **likelihood** and **duration** of delays, enabling smarter planning and smoother operations.

We go beyond standard modeling by:
- Designing a **custom delay score (OAI)** that focuses on delays airlines can control
- Using **SHAP** to explain which features impact predictions the most

---

## Main Idea

To make our predictions, we calculated how much delay typically occurs for each airline at each airport. We did this by defining a custom metric: average delay = total delay divided by total number of flights. This value became our prediction target.

The idea was simple — if we know how an airline usually performs at a certain location, we can estimate the expected delay for a new flight with similar conditions. All the steps, assumptions, and processing logic behind this method are explained in detail in the notebook.

---

## Objectives

- Identify patterns and trends causing delays across months, airlines, and airports
- Predict:
  - Whether a flight will be delayed (classification)
  - How long the delay might be (regression)
- Prioritize actionable delays through **OAI (Operational Adjustability Index)**
- Make predictions explainable with **SHAP**

---

##  Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-007ACC?style=flat&logo=matplotlib&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-Used-blue?style=flat" />
  <img src="https://img.shields.io/badge/SHAP-ExplainableAI-purple?style=flat" />
</p>

---

## Highlights

- Cleaned and explored real-world flight delay data
- Engineered features to capture carrier behavior and airport patterns
- Trained XGBoost models for both regression and classification
- Created a weighted delay score (OAI) to emphasize controllable factors
- Used **SHAP values** for transparent model interpretation

---

