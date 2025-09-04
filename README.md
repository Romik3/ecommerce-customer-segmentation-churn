# E-commerce Customer Segmentation & Churn Prediction with GenAI-Powered Insights

## Project Overview

This project is an end-to-end data science solution designed to provide an e-commerce business with actionable insights into its customer base. By analyzing transactional data, we segment customers into distinct groups, build a machine learning model to predict churn, and leverage Generative AI to brainstorm targeted marketing strategies. The final output is a comprehensive Power BI dashboard that visualizes key business metrics and customer behaviors, transforming raw data into a strategic asset.

![Dashboard Screenshot](dashboard_screenshot.png)

---

## 🎯 Project Objectives

1.  **Customer Segmentation:** Analyze customer purchasing behavior to identify distinct groups using the RFM (Recency, Frequency, Monetary) framework and K-Means clustering.
2.  **Churn Prediction:** Develop a machine learning model to accurately predict the likelihood of a customer churning.
3.  **Actionable Strategy:** Translate data insights into concrete, targeted marketing campaigns by integrating Generative AI for strategic brainstorming.
4.  **Business Intelligence:** Create a dynamic, interactive dashboard for non-technical stakeholders to explore key findings and monitor business health.

---

## 🛠️ Tech Stack & Skills

*   **Programming:** Python
*   **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, imblearn
*   **Database:** SQLite (for EDA)
*   **Machine Learning:** K-Means Clustering, Random Forest, SMOTE (for handling imbalance)
*   **Generative AI:** Google's Gemini (for hypothesis generation & strategy brainstorming)
*   **BI & Visualization:** Power BI
*   **Core Concepts:** Data Cleaning, Feature Engineering, Exploratory Data Analysis (EDA), RFM Analysis, Supervised Learning, Model Evaluation, Data Storytelling

---

## 📂 Project Workflow

The project follows a structured data science lifecycle:

1.  **Data Sourcing & Cleaning:**
    *   Loaded the "Online Retail II UCI" dataset, handling missing values, correcting data types, and removing invalid records.
    *   Engineered a `TotalPrice` feature from `Quantity` and `Price`.

2.  **Exploratory Data Analysis (EDA):**
    *   Utilized **SQLite** to perform initial aggregations and visualized sales trends and top-selling products using Matplotlib and Seaborn.

3.  **Customer Segmentation (RFM & K-Means):**
    *   Calculated **Recency, Frequency, and Monetary (RFM)** scores for each customer.
    *   Applied **K-Means** to segment customers into four distinct personas: **Champions**, **At-Risk Loyalists**, **New & Promising**, and **Potential Loyalists**.

4.  **Churn Prediction Modeling:**
    *   Defined "churn" as any customer who has not made a purchase in the last 90 days.
    *   Built a **Random Forest Classifier** to predict churn based on a customer's purchasing habits, addressing class imbalance using **SMOTE**.

5.  **GenAI-Powered Strategy Brainstorming:**
    *   Used **Google's Gemini** as a strategic partner to generate targeted marketing campaign ideas for retaining "At-Risk Loyalists" and rewarding "Champions".

6.  **Dashboarding & Reporting:**
    *   Exported the final, enriched dataset containing RFM scores, segment labels, and churn probabilities.
    *   Developed an interactive **Power BI dashboard** with three key views: an Executive Overview, a Segment Deep Dive, and a Churn Analysis page.

---

## 📈 Key Results & Insights

*   **Data-Driven Segmentation:** Successfully segmented over 5,000 customers into four actionable groups, revealing that the **"Champions"** segment, despite being small, accounts for a disproportionately large share of total revenue.
*   **Predictive Power:** The churn model can proactively identify customers who are likely to churn, providing the marketing team with an actionable list of high-risk individuals to target with win-back campaigns.
*   **Strategic Roadmapping:** The GenAI integration produced creative marketing strategies tailored to each customer segment, bridging the gap between data analysis and business action.

---

## 🚀 How to Run this Project

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/ecommerce-customer-segmentation-churn.git
    cd ecommerce-customer-segmentation-churn
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Download the dataset:**
    *   Download the "Online Retail II UCI" dataset from the Kaggle or UCI Machine Learning Repository and place the `.csv` file in the project directory.

4.  **Run the Jupyter Notebook:**
    *   Launch Jupyter Notebook and open the `.ipynb` file to view the complete analysis.
    ```bash
    jupyter notebook
    ```
