# Elevate-Task6


a. Use EXTRACT(MONTH FROM order_date) for month
→ Implemented using MONTH(STR_TO_DATE(order_date, '%m/%d/%Y')) because order_date was stored as TEXT.

b. Fixing NULL issue in date extraction
→ Resolved by converting order_date from TEXT to DATE using STR_TO_DATE.

c. Filter records where status = 'received'
→ Done using WHERE status = 'received'.

d. Count number of received orders by month
→ Used COUNT(status) or COUNT(*) grouped by month.

e. Group by extracted month
→ Implemented using GROUP BY MONTH(...) or GROUP BY MONTHNAME(...).

f. Group by year/month
→ Can be done using both YEAR(...) and MONTH(...) in GROUP BY.

g. Use SUM() for revenue
→ Pending. Use SUM(total) or SUM(value) for monthly revenue.

h. Use COUNT(DISTINCT order_id) for volume
→ Pending. Useful for tracking unique orders.

i. Use ORDER BY for sorting
→ Pending. Can sort results by month or total revenue.

j. Limit results for a specific time period
→ Pending. Use WHERE clause with date filters (e.g., month/year).

Dataset Source :- Amazon sales report.csv from kaggle
                2.Order.csv from kaggle
