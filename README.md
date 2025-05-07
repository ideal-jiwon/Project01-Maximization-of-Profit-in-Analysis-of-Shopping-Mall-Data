# 🛍️ Shopping Mall Customer Behavior Analysis

Understand customer behavior patterns, identify peak purchasing times, and build a foundation for personalized marketing strategies.  
— A data analysis project using Python, Pandas, and visualization tools to extract insights from online retail data.

---

## Key Findings

- **82% of total sales come from the UK** — strong regional concentration  
- **November has the highest number of orders in 2011**, followed by December (incomplete)  
- **Peak sales occur during late morning (11 AM – 12 PM)**  
- **Orders begin at 7 AM and sharply decline after 3 PM**  
- **No orders were placed on Saturdays**  
- **Customers often drop off just before checkout** — indicating potential UI/UX friction  

---

## Project Goal

Identify sales patterns and customer drop-off behavior to support data-driven marketing and personalized coupon campaigns.

---

## Analysis Flow

### 1. Data Understanding & Cleansing
- Loaded and inspected `OnlineRetail.csv`
- Removed 135,080 rows with null values (`CustomerID`)
- Filtered invalid transactions (e.g., negative quantity, zero price)

### 2. Exploratory Data Analysis (EDA)
- Identified top-selling items by volume and revenue
- Explored sales trends by:
  - Month
  - Weekday
  - Hour
  - Country

### 3. Customer Segmentation
- Grouped customers by:
  - Purchase frequency
  - Total spending
- Identified **high-value customers (VIPs)**

### 4. Cohort & Retention Analysis
- Monthly cohort grouping using first-purchase month
- Calculated monthly **retention rates**
- Visualized with heatmaps

### 5. Exit Funnel Analysis
- Parsed **web server log-style** data
- Built a **funnel table** to identify common exit pages
- Found key drop-off steps based on session sequences

### 6. Personalized Push Strategy
- Identified **per-user peak purchase hours**
- Proposed **personalized coupon delivery** based on individual behavior

---

## Tools & Tech Used

- **Pandas, NumPy** – data cleaning & transformation  
- **Matplotlib, Seaborn** – visualization & heatmaps  
- **Datetime, Lambda functions** – time feature engineering  
- **Git, Jupyter Notebook** – version control & presentation  

---

## File Structure

