# SQL tips

### Running totals with window functions

`SUM(amount) OVER (ORDER BY order_date)` gives a running total without a self-join.
