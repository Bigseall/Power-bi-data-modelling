# Power-bi-data-modelling
In this project we rebuilt a messy 23-table dataset into a clean data model in Power BI, with core DAX measures and row-level security.

> 📄 Full project explanation (step by step) is on Notion:[https://app.notion.com/p/Power-bi-data-modelling-project-3fc7d086f084805f81e5c3e281dea653?source=copy_link]

---
## Data Model
<img width="1311" height="615" alt="image" src="https://github.com/user-attachments/assets/d6cedd6d-5b8c-4086-8459-5410f4e7d8fa" />
The model is a **galaxy schema**: multiple fact tables sharing common dimensions.

**Dimension tables**
- `dim_customers`
- `dim_products`
- `dim_geo`
- `dim_campaign`
- `dim_order_flags` (junk dimension)
- `dim_date`

**Fact tables**
- `fact_sales`
- `fact_inventory`
- `fact_campaign`
- `fact_promotion_coverage` (factless fact)
- `fact_order_process`
- `fact_sales_targets`
