# Warehouse and Inventory Management Analytics

## Project Overview

This project focuses on solving inventory management challenges using data analytics and machine learning techniques. The objective was to analyze demand patterns, calculate optimal inventory control parameters, and develop predictive models capable of identifying inventory risks before they impact operations.

The project was divided into three analytical components:

| Notebook                              | Objective                                                     |
| ------------------------------------- | ------------------------------------------------------------- |
| LTDemand.ipynb                        | Estimate Lead Time Demand using historical sales transactions |
| SafetyStock & ROP.ipynb               | Calculate Safety Stock and Reorder Point levels               |
| Inventory - Stockout prediction.ipynb | Predict stockout risk using machine learning                  |

## Project Notebooks

### Lead Time Demand Analysis

📓 [View Notebook](https://nbviewer.org/github/chandran1994/Python-Inventory-Analysis-Project/blob/main/LTDemand.ipynb)

### Safety Stock & Reorder Point Analysis

📓 [View Notebook](https://nbviewer.org/github/chandran1994/Python-Inventory-Analysis-Project/blob/main/SafetyStock%20%26%20ROP.ipynb)

### Inventory Stockout Prediction

📓 [View Notebook](https://nbviewer.org/github/chandran1994/Python-Inventory-Analysis-Project/blob/main/Inventory%20-%20Stockout%20prediction.ipynb)

---

# Analytical Workflow

```text
Sales Data
    ↓
Lead Time Demand Analysis
    ↓
Safety Stock Calculation
    ↓
Reorder Point Optimization
    ↓
Stockout Prediction Model
    ↓
Inventory Planning Decisions
```

---

## Data Preparation

The datasets were cleaned and transformed to ensure reliable analytical results.

Key preprocessing activities included:

* Missing value treatment
* Data type optimization
* Feature engineering
* Outlier inspection
* Aggregation of daily demand
* Inventory metric calculations
* Categorical variable encoding

---

## Lead Time Demand Analysis

The first stage of the project focused on estimating Lead Time Demand (LTD), representing the quantity of inventory expected to be consumed while waiting for replenishment.

Historical sales transactions were aggregated into daily demand values and analyzed across multiple time periods. Demand variability was measured to understand consumption uncertainty and identify products with unstable demand patterns.

### Core Calculation

```python
Lead Time Demand = Average Daily Demand × Lead Time
```

This analysis established the inventory consumption baseline required for replenishment planning.

---

## Safety Stock & Reorder Point Optimization

Using Lead Time Demand results, inventory buffers were calculated to reduce stockout risk while maintaining target service levels.

Safety Stock calculations incorporated demand variability and lead time uncertainty.

### Core Calculations

```python
Safety Stock = Z × σLTD

Reorder Point = Lead Time Demand + Safety Stock
```

Where:

* Z = Service level factor
* σLTD = Standard deviation of Lead Time Demand

The analysis identified optimal inventory thresholds for replenishment decisions and inventory control.

---

## Inventory Stockout Prediction

The final stage of the project focused on predicting future stockout risk using machine learning.

Inventory, demand, and operational features were analyzed to identify variables associated with stockout events.

The dataset was prepared using feature engineering and categorical encoding techniques before model development.

### Machine Learning Pipeline

```text
Data Cleaning
      ↓
Feature Engineering
      ↓
Train-Test Split
      ↓
Model Training
      ↓
Prediction
      ↓
Model Evaluation
```

The resulting classification model predicts whether a product is likely to experience a stockout, allowing planners to take corrective actions before inventory shortages occur.

---

## Business Value

This project demonstrates how inventory analytics can support operational decision-making by :

* Reducing stockout risk
* Improving inventory availability
* Supporting replenishment planning
* Optimizing inventory investment
* Enhancing service-level performance
* Enabling proactive inventory management

---
