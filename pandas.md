# pandas tips

### Read only the columns you need

`pd.read_csv(path, usecols=["id", "amount"])` cuts memory use a lot on wide files.

### Chunk large CSVs

`pd.read_csv(path, chunksize=100_000)` returns an iterator, so a file bigger than RAM can still be processed.
