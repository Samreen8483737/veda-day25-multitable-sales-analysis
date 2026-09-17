# Day 25: Multi-Table Sales Analysis

## Objective
Apply end-to-end relational analysis by combining distinct Orders, Products, and Customers tables via SQL `JOIN` operations to facilitate comprehensive business intelligence reporting in Power BI.

## Technical Implementation
* **SQL:** Utilized Python's `sqlite3` to architect a relational database and executed a master `INNER JOIN` query to consolidate normalized data. Computed dynamic revenue columns (Quantity * Price) at runtime.
* **Power BI:** Ingested the consolidated CSV output to build interactive visualizations tracking revenue by region, product category, and individual client contribution.
* **Data Validation:** Implemented pre- and post-join aggregation checks to ensure no double-counting or row duplication occurred during the one-to-many table merges. 

## Key Business Insights
1. **Top Revenue Driver:** The North region is the most valuable territory, generating $9,000 in total sales.
2. **Product Performance:** The Electronics category significantly outperforms Furniture in revenue generation ($15,900 vs $1,500), despite Furniture having a higher individual transaction volume.
3. **Client Concentration Risk:** Acme Corp accounts for over 50% of total revenue ($9,000 of the $17,400 total). The business is currently heavily reliant on this single relationship.
4. **Volume vs. Margin:** While Laptops drive high revenue per unit ($1,200), Monitors matched their total revenue contribution by selling at a much higher volume.
5. **Join Validation:** The total aggregated sales in the dashboard ($17,400) perfectly matches the expected sum of the raw SQL output, confirming flawless relational joins.
