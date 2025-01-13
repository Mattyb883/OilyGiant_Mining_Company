# Oil Well Development: Finding the Best Region

## Project Overview

This project focuses on identifying the most profitable region for developing new oil wells for the **OilyGiant mining company**. Using predictive modeling, profit calculations, and risk analysis, we analyzed data from three regions to determine the optimal location for maximizing revenue and minimizing risk.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objective](#business-objective)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Findings](#findings)
- [Conclusion and Recommendations](#conclusion-and-recommendations)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)

---

## Business Objective

The primary objective was to:
1. Build predictive models for oil well reserves.
2. Calculate profit and evaluate risks for each region.
3. Recommend the region with the highest profitability and lowest risk.

---

## Data Description

The dataset includes geological exploration data for three regions:

- **Columns**:
  - `id`: Unique oil well identifier.
  - `f0`, `f1`, `f2`: Features describing geological properties (exact meanings are unimportant).
  - `product`: Oil reserves in thousand barrels.
- **Conditions**:
  - A study of 500 points per region was conducted.
  - Development budget: $100 million USD for 200 wells.
  - Revenue per thousand barrels: $4,500 USD.
  - Risk tolerance: Maximum 2.5% probability of losses.

---

## Methodology

1. **Data Preparation**:
   - Cleaned data and removed duplicates.
   - Calculated break-even reserve volume for profitability.
2. **Model Training**:
   - Used linear regression models to predict reserves.
   - Evaluated model performance using RMSE and average reserves.
3. **Profit Calculation**:
   - Selected the top 200 wells per region based on predictions.
   - Calculated profit using actual reserves.
4. **Risk Analysis**:
   - Applied bootstrapping with 1,000 simulations to estimate profit variability and risk of losses.

---

## Findings

- **Break-Even Volume**: 111.11 thousand barrels per well.
- **Region Performance**:
  - **Region 0**: Avg Profit = $25.64M, Risk = 4.50%.
  - **Region 1**: Avg Profit = $18.27M, Risk = 10.25%.
  - **Region 2**: Avg Profit = $27.48M, Risk = 3.80%.

---

## Conclusion and Recommendations

1. **Primary Recommendation**: Focus on **Region 2** for oil well development due to the highest average profit and lowest risk of losses.
2. **Backup Option**: Consider **Region 0** as a secondary candidate.
3. **Exclude Region 1**: Low average profit and high risk of losses make it unsuitable for development.

---

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical computations.
  - `sklearn`: Machine learning and evaluation.
  - `matplotlib`: Data visualization.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/oil-well-development.git
   cd oil-well-development
