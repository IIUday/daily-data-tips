# Python tips

### Use pathlib for file paths

`Path("data") / "sales.csv"` works on every OS and reads better than string concatenation.

### f-string number formatting

`f"{value:,.2f}"` prints 1234567.891 as 1,234,567.89.
