Sales Trend Analysis Project:

Overview:

This project provides a complete Oracle SQL solution for analyzing monthly sales trends, including revenue and order volume metrics. The implementation covers database table creation, sample data insertion, and analytical queries with all requested features.

Features:

  - Complete SQL Implementation:
  - Table creation for sales data
  - Sequence generation for order IDs
  - Sample data insertion (10 records)
  - Comprehensive sales analysis query

  - Analysis Capabilities:
  - Monthly revenue totals (SUM)
  - Order volume counts (COUNT DISTINCT)
  - Average order value calculation
  - Time period filtering
  - Chronological sorting

SQL Features Implemented:

1. Date Extraction (EXTRACT(MONTH/YEAR FROM date))
2. Grouping (GROUP BY year and month)
3. Aggregation (SUM() for revenue)
4. Counting (COUNT(DISTINCT) for order volume)
5. Sorting (ORDER BY year and month)
6. Date Filtering (specific time periods)

Installation:

1. Ensure you have Oracle Database installed
2. Run the complete SQL script in your Oracle SQL client
3. The script will:
   - Create the online_sales table
   - Create the order_id_seq sequence
   - Insert 10 sample records
   - Execute the sales analysis query

Usage:

After running the script, you can:

1. Modify the date range in the WHERE clause to analyze different periods
2. Add additional metrics to the SELECT clause
3. Adjust the GROUP BY to analyze at different time granularities

Sample Output:

SALES_YEAR SALES_MONTH MONTH_NAME TOTAL_REVENUE ORDER_VOLUME AVG_ORDER_VALUE
---------- ----------- ---------- ------------- ------------ ---------------
      2022           3 MAR              225.50            2          112.75
      2022           4 APR              325.25            2          162.63
      2022           5 MAY               90.75            1           90.75
      2023           1 JAN              400.50            2          200.25
      2023           2 FEB               95.30            1           95.30
      2023           3 MAR              326.00            2          163.00
      

Customization:

To analyze different time periods, modify the WHERE clause:

WHERE order_date BETWEEN TO_DATE('YYYY-MM-DD', 'YYYY-MM-DD') 
                   AND TO_DATE('YYYY-MM-DD', 'YYYY-MM-DD')


