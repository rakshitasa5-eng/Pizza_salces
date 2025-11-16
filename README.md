### Pizza Salces

-- Project: Pizza Sales Analysis with Power BI SQL Quarys 

-- Objective: Generate insights from pizza_sales dataset using DAX and Power BI visuals.

-- Key Metrics:
SELECT
    SUM(total_price)     AS Total_Revenue,       -- 817.86K
    
    AVG(order_value)     AS Avg_Order_Value,     -- 38.31
    
    SUM(total_pizzas)    AS Total_Pizzas_Sold,   -- 49,574
    
    COUNT(order_id)      AS Total_Orders,        -- 21,350
    
    (SUM(total_pizzas) / COUNT(order_id))
                        AS Avg_Pizzas_Per_Order; -- 2.32

-- Insights:

    -- 1. Busiest Days & Times: Weekends and Evenings show peak sales.

    -- 2. Monthly Trend: Orders consistently higher from Jan–Jul.

    -- 3. Category Performance: Classic pizzas contribute maximum revenue.

    -- 4. Size Performance: Large pizzas generate the highest revenue share.

    -- 5. Best Sellers: Top pizzas identified by revenue, quantity, and orders.

    -- 6. Worst Sellers: Bottom 5 pizzas listed for optimization.

-- Visuals Used:

    -- Bar charts, line charts, donut charts, KPI cards, and matrix tables.

-- Tools:
    -- Power BI Desktop, DAX Measures, Data Modeling.
