# pandas tips

### Read only the columns you need

`pd.read_csv(path, usecols=["id", "amount"])` cuts memory use a lot on wide files.

### Chunk large CSVs

`pd.read_csv(path, chunksize=100_000)` returns an iterator, so a file bigger than RAM can still be processed.

### Use category dtype for repeated strings

`df["city"] = df["city"].astype("category")` can shrink memory 10x when a column has few unique values.
