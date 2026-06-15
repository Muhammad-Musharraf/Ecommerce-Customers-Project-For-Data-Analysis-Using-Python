# 🛒 Ecommerce Customers — Data Analysis Project

A Python-based Exploratory Data Analysis (EDA) project that uncovers customer behavior patterns, spending trends, and engagement insights from an ecommerce dataset of 500 customers.

---

## 📌 Project Overview

This project performs a thorough EDA on an ecommerce customers dataset to answer real business questions around customer spending, platform engagement, membership behavior, and demographic segmentation. The analysis combines data filtering, grouping, and rich visualizations to surface actionable insights for data-driven decision-making.

---

## 📁 Repository Structure

```
Ecommerce-Customers-Project-For-Data-Analysis-Using-Python/
│
├── Dataset/
│   └── Ecommerce Customers.xlsx       # Source dataset (500 customers, 8 features)
│
├── Project/
│   └── Project Of Ecommerce Customer (1).ipynb   # Main Jupyter Notebook
│
├── LICENSE
└── README.md
```

---

## 📊 Dataset Description

The dataset contains **500 records** and **8 columns** describing ecommerce customer attributes:

| Column | Description |
|---|---|
| `Email` | Customer email address |
| `Address` | Customer physical address |
| `Avatar` | Customer avatar color preference |
| `Avg. Session Length` | Average session length (minutes) |
| `Time on App` | Time spent on the mobile app (minutes) |
| `Time on Website` | Time spent on the website (minutes) |
| `Length of Membership` | How long the customer has been a member (years) |
| `Yearly Amount Spent` | Total yearly spending by the customer ($) |

- **Rows:** 500  
- **Missing Values:** None  
- **Duplicates:** None  

---

## 🔍 Key Analyses Performed

### Data Quality Checks
- Shape, data types, and statistical summary (`describe()`)
- Null value and duplicate detection
- Unique value counts per column

### Data Filtering (Business Questions)
- How many customers use the `SlateBlue` avatar with membership longer than 4 years?
- Emails of customers with yearly spending > $300 and membership < 2 years
- Addresses and emails of customers spending > 10 minutes on the app with a `GreenYellow` avatar
- Count of customers spending > 2 minutes on the website
- Customers spending > 30 minutes on the website AND yearly amount > $500
- Customers with membership ≥ 4 years AND yearly spending > $500

### Grouping & Aggregation
- Customer distribution by Avatar and Email
- Customer distribution by Avatar and Address

### Data Visualization

| Plot | Purpose |
|---|---|
| Scatter — Membership Length vs Yearly Spend | Relationship between loyalty and revenue |
| KDE — Membership Length | Distribution of membership durations |
| Histogram + KDE — Membership Length | Frequency distribution with density curve |
| KDE — Yearly Amount Spent | Spending distribution shape |
| Histogram + KDE — Yearly Amount Spent | Spending frequency analysis |
| Scatter — Time on App vs Time on Website | Platform engagement comparison |
| Histogram + KDE — Avg. Session Length | Session length distribution |
| Scatter — Avg. Session Length vs Membership Length | Session behavior by tenure |
| Scatter — Avg. Session Length vs Time on App | App usage vs session length |
| Pair Plot (all features) | Full feature correlation overview |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| Pandas | Data loading, filtering, grouping |
| NumPy | Numerical operations |
| Matplotlib | Base plotting |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Interactive analysis environment |
| openpyxl / xlrd | Reading `.xlsx` files |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.7+ and the following libraries installed:

```bash
pip install pandas numpy matplotlib seaborn openpyxl jupyter
```

### Run the Notebook

```bash
# Clone the repository
git clone https://github.com/Muhammad-Musharraf/Ecommerce-Customers-Project-For-Data-Analysis-Using-Python.git

# Navigate into the project
cd Ecommerce-Customers-Project-For-Data-Analysis-Using-Python

# Launch Jupyter Notebook
jupyter notebook "Project/Project Of Ecommerce Customer (1).ipynb"
```

> **Note:** Ensure the dataset path in the notebook (`Ecommerce Customers.xlsx`) points to the `Dataset/` folder, or copy the file into the same directory as the notebook before running.

---

## 💡 Key Findings

- **Membership length and yearly spending are positively correlated** — longer-tenured customers tend to spend more annually, highlighting the value of retention strategies.
- **Mobile app engagement** is a stronger indicator of spending than website time, suggesting investment in app experience may drive more revenue.
- **Customer segmentation** using avatar, session length, and spending thresholds enables targeted marketing to high-value customer groups.
- **Average session length** shows a relatively normal distribution, providing a reliable baseline for engagement benchmarking.
- **Most customers** fall within a yearly spend range that can be used to define tiered loyalty programs.

---

## 📌 Conclusion

This project demonstrates how EDA techniques can transform raw ecommerce data into actionable business intelligence. By combining filtering, grouping, and visualization, the notebook surfaces patterns in customer behavior that support decisions around product development, marketing campaigns, and platform investment.

---

## 📄 License

This project is licensed under the terms of the [LICENSE](LICENSE) file included in this repository.

---

## 🙋 Author

**Muhammad Musharraf**  
[GitHub Profile](https://github.com/Muhammad-Musharraf)
