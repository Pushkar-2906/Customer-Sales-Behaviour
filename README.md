# Customer-Sales-Behaviour

# 🛍️ Customer Shopping Behavior Analysis

An end-to-endData Analytics project focused on analyzing customer shopping patterns, purchasing behavior, product performance, customer segmentation, and revenue trends using*Python, SQL, PostgreSQL, and Power BI.

The project transforms raw transactional data into meaningful business insights that can support data-driven decision-making.

---

 📌 Overview

Understanding customer behavior is essential for improving sales, customer retention, marketing strategies, and product performance.

This project analyzes a dataset containing **3,900 customer purchase records across 18 attributes**. The analysis covers customer demographics, purchase details, discounts, reviews, subscriptions, shipping methods, purchase frequency, and customer loyalty.

The project follows a complete analytics workflow:

**Raw Data → Python EDA → Data Cleaning → SQL Analysis → Business Insights → Power BI Dashboard → Report & Presentation**

---

 📂 Dataset

The dataset contains **3,900 records and 18 columns** related to customer shopping behavior.

 Key Features

| Category             | Features                                              |
| -------------------- | ----------------------------------------------------- |
| Customer Information | Age, Gender, Location, Subscription Status            |
| Purchase Details     | Item Purchased, Category, Purchase Amount             |
| Product Information  | Season, Size, Color                                   |
| Shopping Behavior    | Discount Applied, Promo Code Used, Previous Purchases |
| Customer Feedback    | Review Rating                                         |
| Delivery             | Shipping Type                                         |
| Purchase Behavior    | Frequency of Purchases                                |

The dataset initially contained **37 missing values in the Review Rating column**, which were handled during the data-cleaning stage.

---

 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **Jupyter Notebook**
* **PostgreSQL**
* **SQL**
* **Power BI**
* **Gamma** for presentation development
* **Microsoft Excel/CSV** for dataset handling

---

 🔄 Project Workflow

 1. Data Loading

The customer shopping dataset was imported into Python using **Pandas**.

Initial inspection was performed to understand:

* Dataset structure
* Data types
* Number of records
* Missing values
* Statistical distributions
* Categorical variables

---

 2. Exploratory Data Analysis

Exploratory analysis was performed to identify patterns and trends within the dataset.

The analysis examined:

* Customer demographics
* Purchase amounts
* Product categories
* Customer ratings
* Discounts
* Subscription status
* Shipping methods
* Purchase frequency
* Customer loyalty

---

 3. Data Cleaning

The dataset was prepared for further analysis by performing several preprocessing operations.

Key cleaning activities included:

* Identifying missing values
* Handling missing Review Rating values
* Standardizing column names
* Checking data consistency
* Removing redundant information
* Preparing additional analytical features

Missing review ratings were imputed using the **median rating of the corresponding product category**.

---

 4. Feature Engineering

Additional features were created to support deeper analysis.

#### Age Group

Customer ages were categorized into groups to analyze revenue and purchasing behavior across different age segments.

Purchase Frequency

Purchase-related information was transformed into a frequency-based feature to support customer behavior analysis.

---

🗄️ SQL Analysis

The cleaned dataset was imported into **PostgreSQL** for structured business analysis.

SQL queries were used to answer important business questions such as:

 Business Questions

1. Which gender contributes more revenue?
2. Which customers use discounts but still spend above average?
3. Which products have the highest average ratings?
4. How does average purchase value differ between Standard and Express shipping?
5. How do subscribers compare with non-subscribers in terms of spending and revenue?
6. Which products have the highest discount dependency?
7. How many customers belong to New, Returning, and Loyal segments?
8. What are the top products within each category?
9. Are repeat buyers more likely to subscribe?
10. Which age group contributes the highest revenue?

---

 📊 Power BI Dashboard

An interactive **Power BI dashboard** was created to communicate the results visually.

Dashboard KPIs

* **Total Customers:** 3.9K
* **Average Purchase Amount:** $59.76
* **Average Review Rating:** 3.75

 Dashboard Visualizations

The dashboard includes:

* Subscription status distribution
* Revenue by category
* Sales by category
* Revenue by age group
* Sales by age group
* Customer filtering by gender
* Category filtering
* Shipping type filtering
* Subscription filtering

The dashboard allows users to interactively filter the data and explore customer behavior from different perspectives.

---

📈 Key Results

The analysis produced several important findings.

### Customer Segmentation

Customers were divided into three segments:

| Segment   | Customers |
| --------- | --------: |
| Loyal     |     3,116 |
| Returning |       701 |
| New       |        83 |

The Loyal segment represents the largest group in the dataset.

#Top-Rated Products

The products with the highest average ratings included:

| Product | Average Rating |
| ------- | -------------: |
| Gloves  |           3.86 |
| Sandals |           3.84 |
| Boots   |           3.82 |
| Hat     |           3.80 |
| Skirt   |           3.78 |

 Revenue by Age Group

| Age Group   | Revenue |
| ----------- | ------: |
| Young Adult |  62,143 |
| Middle-aged |  59,197 |
| Adult       |  55,978 |
| Senior      |  55,763 |

The Young Adult segment generated the highest revenue among the analyzed age groups.

Shipping Analysis

The average purchase amounts were approximately:

* **Standard:** 58.46
* **Express:** 60.48

Express shipping showed a slightly higher average purchase value.

Discount-Dependent Products

The products with the highest discount rates included:

* Hat
* Sneakers
* Coat
* Sweater
* Pants

This highlights the importance of monitoring discount strategies and their impact on sales and profitability.

---

 💡 Business Recommendations

Based on the analysis, several business strategies can be considered.

 1. Increase Subscription Adoption

Introduce exclusive benefits and targeted offers to encourage suitable non-subscribers to join subscription programs.

 2. Strengthen Customer Loyalty

Reward repeat customers through loyalty programs and personalized offers to maintain long-term engagement.

 3. Optimize Discount Strategies

Monitor products that frequently rely on discounts and balance promotional activity with profitability.

 4. Promote High-Performing Products

Give greater visibility to products with strong ratings and high purchase volumes.

 5. Use Targeted Marketing

Develop age-specific and customer-segment-specific campaigns based on revenue contribution and purchasing behavior.

6. Analyze Shipping Preferences

Further evaluate the relationship between shipping options and customer spending to identify opportunities for improving the shopping experience.

---

 📁 Project Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── customer_shopping_behavior.csv
│
├── DATA.py
│
├── notebooks_Intro.ipynb
│
├── cust.sql
│
├── final_Queries.sql
│
├── PowerBI/
│   └── Customer_Behavior_Dashboard.pbix
│
├── Report/
│   └── Customer_Shopping_Behavior_Analysis.pdf
│
├── Presentation/
│   └── Customer_Shopping_Behavior_Analysis.pptx
│
└── README.md
```

---

 ▶️ How to Run

 Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/customer-shopping-behavior-analysis.git
```

 Step 2: Navigate to the Project

```bash
cd customer-shopping-behavior-analysis
```

 Step 3: Install Required Python Library

```bash
pip install pandas
```
 Step 4: Run the Python Analysis

Make sure `customer_shopping_behavior.csv` is located in the same directory as the Python script.

Run:

```bash
python DATA.py
```

Alternatively, open:

```text
notebooks_Intro.ipynb
```

in Jupyter Notebook or JupyterLab.

 Step 5: Run SQL Analysis

Import the cleaned dataset into PostgreSQL and execute the SQL scripts:

```text
cust.sql
final_Queries.sql
```

These queries generate the business insights used in the project.

 Step 6: Open the Power BI Dashboard

Open the `.pbix` file using **Microsoft Power BI Desktop** and refresh the dataset if required.

---

 📊 Skills Demonstrated

This project demonstrates practical skills in:

* Data Cleaning
* Exploratory Data Analysis
* Data Preprocessing
* Feature Engineering
* Python & Pandas
* SQL
* PostgreSQL
* Business Analytics
* Customer Segmentation
* Revenue Analysis
* Data Visualization
* Power BI Dashboard Development
* Business Insight Generation
* Data-Driven Decision Making

---

 🎯 Project Objective

The objective of this project is to demonstrate how a Data Analyst can take a raw customer dataset, clean and explore the data, perform SQL-based analysis, build an interactive dashboard, and convert analytical findings into practical business recommendations.

It showcases an end-to-end **Data Analytics workflow** from raw data to business intelligence.

---

 👤 Author

Pushkar Ashok Mhaske

Computer Engineering Student | Data Analytics Enthusiast

 Areas of Interest

* Data Analytics
* Business Analytics
* SQL
* Python
* Power BI
* Business Intelligence
* Data-Driven Decision Making

