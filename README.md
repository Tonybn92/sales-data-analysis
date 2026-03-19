📊 Sales Data Analysis — Exploratory Data Analysis (EDA)
🧠 Project Overview

This project is part of my Data Analyst portfolio, where I apply end-to-end data analysis techniques using the Superstore Sales dataset.

The goal of this project is to simulate a real-world data analysis workflow, covering data exploration, data quality validation, statistical analysis, visualization, and business insights generation.

🧱 Project Structure
sales-data-analysis
│
├── data/
├── notebooks/
├── sql/
├── dashboard/
└── README.md
🛠️ Tools & Technologies

Python
pandas
numpy
matplotlib
seaborn
Jupyter Notebook (VS Code)
Git & GitHub

📥 Data Loading

The dataset was loaded using pandas, handling encoding issues:

pd.read_csv("../data/Superstore.csv", encoding="windows-1252")
🔍 Exploratory Data Analysis (EDA)
1️⃣ Dataset Overview

Initial exploration included:

Dataset shape
Column names
Data types
Basic statistics

Key findings:

The dataset contains 9994 rows and 21 columns

Data includes both categorical and numerical variables

2️⃣ Data Types & Structure

Numerical variables: Sales, Profit, Quantity, Discount

Categorical variables: Category, Region, Segment, Ship Mode, etc.

3️⃣ Missing Values

No significant missing values were found in the dataset

4️⃣ Duplicate Check

No fully duplicated rows were found

The dataset contains unique records for each transaction

📊 Categorical Variables Analysis
Tools used:

unique()

nunique()

value_counts()

value_counts(normalize=True)

🪑 Category

Furniture

Office Supplies

Technology

Insight:

The business operates across multiple product types, covering office essentials, furniture, and technology products.

🌎 Region

West: 3203

East: 2848

Central: 2323

South: 1620

Insight:

The West region is the most active market, while the South region shows lower activity levels.

👥 Segment

Consumer: ~52%

Corporate: ~30%

Home Office: ~18%

Insight:

The business depends heavily on individual consumers, as they represent the majority of transactions.

🚚 Ship Mode

Standard Class dominates

Insight:

Customers prefer cost-effective shipping over faster delivery options.

📊 Numerical Variables Analysis
Variables analyzed:

Sales

Profit

Quantity

Discount

💰 Sales

Mean: ~229

Max: ~22,638

Insight:

Most transactions are low-value, but there are occasional high-value sales.

📉 Profit

Mean: ~28

Min: ~-6599

Max: ~8399

Insight:

There are significant losses in some transactions, indicating potential issues with pricing or discounts.

⚠️ Discount

Maximum discount: 80%

🔥 High Discount Impact Analysis

Further analysis was performed on transactions with 80% discount:

Total Sales: 16,963

Percentage of total sales: 0.74%

Number of transactions: 300

Total Profit: -30,539

Insight:

A very small portion of transactions generates a disproportionately large amount of losses.

This suggests that high discount levels are negatively impacting profitability and may not be a sustainable strategy.

📊 Data Visualization & Outlier Detection
Techniques used:

Boxplots

Histograms

Logarithmic scaling (plt.xscale('log'))

Data filtering for better visualization

Key Findings

The dataset is highly skewed (right-skewed distribution)

Most values are concentrated at lower ranges

There are significant outliers in both Sales and Profit

📊 Distribution Insights

Most sales are small, with a few very large transactions

Most profits are close to zero

Some transactions generate large losses and large gains

Insight:

The business relies on many small transactions, while a small number of large transactions significantly impact overall performance.

🧠 Key Learnings

Performed full exploratory data analysis (EDA)

Identified data distribution patterns and outliers

Analyzed categorical and numerical variables

Detected business issues related to discount strategies

Applied visualization techniques to better understand data behavior

Transformed raw data into meaningful business insights

🚀 Next Steps

The next phase of the project will focus on business-level analysis, including:

Sales by Category

Sales by Region

Profitability by Segment

Identifying loss-generating products or segments

Building visual insights for dashboards (Power BI)

🎯 Project Outcome

This project demonstrates the ability to:

Work with real-world datasets

Perform structured data analysis

Extract actionable business insights

Communicate findings effectively