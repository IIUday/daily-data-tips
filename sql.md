# SQL tips

### Running totals with window functions

`SUM(amount) OVER (ORDER BY order_date)` gives a running total without a self-join.

### COUNT(*) vs COUNT(column)

`COUNT(*)` counts rows, `COUNT(col)` skips NULLs. Mixing them up silently changes averages.

### Filter groups with HAVING

`WHERE` filters rows before grouping, `HAVING` filters after. `HAVING SUM(sales) > 1000` keeps only big groups.
