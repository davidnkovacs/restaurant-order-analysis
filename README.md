# Restaurant Order Analysis: Data Exploration & Insights

## Project Overview

This project involves analyzing a multi-table dataset from a fictional restaurant to uncover insights into customer behavior, menu performance, and revenue drivers. Using **SQL**, the goal was to transform raw data into actionable intelligence for the restaurant's management team.

The analysis focuses on answering two primary questions:

1. **Which menu items are driving the most (and least) revenue?**
2. **What does the typical customer "basket" look like?**

---

## Tech Stack & Skills

* **Tool:** MySQL / PostgreSQL (or your specific SQL flavor)
* **Skills:** * Data Cleaning & Type Casting
* Table Joins (`LEFT`, `INNER`)
* Aggregations (`COUNT`, `SUM`, `AVG`)
* Filtering & Sorting
* Common Table Expressions (CTEs)



---

## Dataset Structure

The project utilizes two main tables:

1. **`menu_items`**: Contains details on item names, categories (Italian, Mexican, etc.), and prices.
2. **`order_details`**: Contains transactional data, including order IDs, item IDs, and timestamps.

---

## Key Analysis Steps

### 1. Menu Exploration

I began by profiling the menu to understand the price range and cuisine variety.

* **Total Items:** 32 items across 4 categories.
* **Price Range:** $5.00 to $19.95.
* **Top Insight:** Italian food represents the most expensive category on average.

### 2. Order Volume & Timing

Analyzed the `order_details` table to find patterns in customer traffic.

* **Total Orders:** 5,370 unique orders.
* **Volume:** The dataset covers three months of activity.
* **Peak Items:** Identifying which specific items appear most frequently in transaction logs.

### 3. Deep Dive: Customer Behavior

By joining the tables, I analyzed which cuisines and items generated the highest spend.

* **Top 5 Highest Spend Orders:** Discovered specific high-value transactions and the items within them.
* **Cuisine Popularity:** Mexican items were frequently ordered, but Italian items drove higher revenue per order.

---

## Key Findings

* **The "Big Winners":** The **Hamburger** was the most frequently ordered item, while **Eggplant Parmesan** (Italian) contributed significantly to total revenue.
* **Underperformers:** Specific items like the **Chicken Tacos** had surprisingly low order volume compared to other Mexican dishes.
* **Basket Analysis:** High-spend orders almost always included a combination of expensive Italian entrees and multiple sides, suggesting that "Dinner for Two" or "Family Style" ordering is a key revenue driver.

---

## Conclusion & Recommendations

1. **Promote Italian Cuisine:** Since Italian items have the highest margins, the restaurant should feature these in marketing or "Chef's Specials."
2. **Menu Optimization:** Consider removing or rebranding the lowest-performing items to reduce inventory waste.
3. **Bundle Deals:** Create "Combo" deals for the most popular items (like the Hamburger) to increase the average transaction value.

---

## How to Run This Project

1. Download the `.sql` files provided in this repository.
2. Import the datasets into your SQL Workbench.
3. Execute the queries in order to replicate the analysis.
