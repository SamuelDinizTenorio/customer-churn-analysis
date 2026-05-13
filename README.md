# 📊 Python Insights - Churn Data Analysis

![Python](https://img.shields.io/badge/python-3.12+-blue.svg?logo=python&logoColor=white)
![Venv](https://img.shields.io/badge/venv-isolated-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)
![Platform](https://img.shields.io/badge/OS-Linux%20%7C%20Windows-lightgrey.svg)

This project was developed during Lesson 2 of the Python Immersion course by **Hashtag Treinamentos**. It involves analyzing a dataset of over 800,000 customers. The primary objective is to identify the reasons behind customer churn and propose data-driven solutions to mitigate it.

## 🚀 Technologies

- **Python 3.12+**: Core language.
- **Pandas**: Data manipulation, cleaning, and preprocessing.
- **Plotly**: Interactive data visualization.
- **Virtualenv (venv)**: Development environment isolation.
- **Jupyter Notebook (.ipynb)**: Development environment for exploratory data analysis (EDA).

## 📦 Environment Setup

It is recommended to use a virtual environment to install the dependencies listed in `requirements.txt`.

```bash
# 1. Create the virtual environment
python3 -m venv venv

# 2. Activate the environment
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate   # Windows

# 3. Install dependencies
pip install -r requirements.txt
```

## 🛠️ Project Pipeline (Workflow)

1. **Data Ingestion & Cleaning**:Loading the dataset and dropping irrelevant features (such as CustomerID).

2. **Data Wrangling**: Identifying and handling missing values (NaN) to ensure analytical integrity.

3. **Baseline Analysis**: Evaluating the current churn rate (initial benchmark at ~56%).

4. **Exploratory Data Analysis (EDA)**: Utilizing interactive charts to correlate variables with the churn status.

5. **Key Insights Identification**:

- **Contract Type**: 100% churn rate observed for monthly contracts.
- **Support Overhead**: Customers with more than 4 call center interactions churned..
- **Payment Latency**: Overdue payments exceeding 20 days resulted in total churn.

## 💡 Business Insights & Action Plan

Based on the data analysis, the following strategic actions are proposed to mitigate churn. If implemented, the projected churn rate could drop from 56% to approximately 18%:

- **Annual/Quarterly Plan Incentives**: Offer targeted discounts to migrate customers from monthly contracts to longer-term commitments.
- **Customer Support Optimization**: Implement a trigger-based alert system for customers who contact the call center more than 3 times, ensuring priority resolution.
- **Credit Recovery Strategy**: Establish proactive billing and negotiation workflows before a payment delay exceeds the 20-day critical threshold.

## 📂 Project Structure

- **main.ipynb**: Core Jupyter Notebook containing the end-to-end analysis and visualization logic.
- **cancelamentos.csv**: Example database file used in class (Portuguese).
- **requirements.txt**: Dependency manifest for environment replication (Pandas, Plotly, etc).
- **.gitignore**: Configured to exclude venv/.