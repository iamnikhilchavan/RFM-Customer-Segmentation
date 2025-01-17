# Customer Segmentation and CLTV Estimation

This project demonstrates customer segmentation using RFM Analysis and Customer Lifetime Value (CLTV) estimation to provide valuable insights into customer behavior and improve business decision-making for e-commerce.

---

## Overview

The objective of this project is to:
1. Perform customer segmentation using **RFM Analysis** (Recency, Frequency, Monetary Value).
2. Estimate **Customer Lifetime Value (CLTV)** using machine learning algorithms such as BetaGeoFitter and Gamma-Gamma Fitter.
3. Use segmentation to inform targeted marketing strategies and improve revenue generation.

## Data Source

The dataset, obtained from the **UCI Repository** and **Kaggle**, contains e-commerce transactional data from 2009 to 2010, including details such as:
- Customer ID, Invoice Number, Stock Code
- Purchase Date, Country
- Transaction Quantity, Unit Price

---

## Methodology

1. **Exploratory Data Analysis (EDA)**:
   - Analyzed customer demographics and spending patterns.
   - Observed skewness in price distribution and geographic concentration of customers (majority in the UK).

2. **RFM Analysis**:
   - Extracted Recency, Frequency, and Monetary Value attributes.
   - Plotted distribution to understand customer behavior.
   - Performed manual segmentation and observed dominant segments (e.g., Champions and Hibernating customers).

3. **CLTV Estimation**:
   - Used probabilistic models (**BetaGeoFitter** and **Gamma-Gamma Fitter**) to estimate CLTV.
   - Combined Recency, Frequency, and Monetary Value with predicted CLTV for better customer segmentation.

4. **Clustering**:
   - Applied **K-Means Clustering** on RFM and CLTV data.
   - Used the Elbow Method to determine the optimal number of clusters.
   - Visualized clusters using scatter plots and a Relative Importance Heatmap.

---

## Key Takeaways

- **RFM Analysis**:
  - Identified bulk-order customers (high monetary value, low frequency).
  - Found frequent but low-value customers for loyalty programs.

- **CLTV-Based Segmentation**:
  - Segmented customers into actionable clusters for targeted marketing.
  - Highlighted areas for improvement in customer retention and acquisition.

---

## Results

- Developed a heatmap showing the relative importance of Recency, Frequency, and Monetary Value across clusters.
- Segmented customers into 5 meaningful groups:
  - High-Value Customers (Champions)
  - At-Risk Customers
  - Loyal Customers
  - New Customers
  - Hibernating Customers

---

## Conclusion

The combination of RFM and CLTV-based segmentation provides a more comprehensive and actionable approach to customer segmentation. This approach helps businesses prioritize high-value customers and focus on retention strategies for at-risk customers. Future steps could include integrating hierarchical clustering for further optimization.

---

## Dependencies

Install the necessary dependencies using the provided `requirements.txt` file:
```bash
pip install -r requirements.txt
```
## Usage

To use this repository, follow these steps:

1. **Clone the repository**:
```bash
git clone https://github.com/iamnikhilchavan/RFM-Customer-Segmentation.git
cd <repository_folder>
```

2. **Set up the Python environment**:

  i. **Create and activate a virtual environment**:
```bash
python -m venv .env

source .env/bin/activate  # For MacOS/Linux
.env\Scripts\activate     # For Windows
```
  ii. **Install the required dependencies**:
```bash
pip install -r requirements.txt
```
3. **Run the Jupyter Notebook**:
```bash
jupyter notebook
```
open the .ipynb file and execute the cells in the notebook. 


