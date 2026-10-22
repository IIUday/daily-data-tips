# Power BI tips

### Keep a separate date table

Mark a dedicated calendar table as the date table so time intelligence functions like `TOTALYTD` work reliably.

### Measures over calculated columns

Calculated columns are stored per row and bloat the model; measures are computed on the fly for the current filter.
