# pandas tips

### Read only the columns you need

`pd.read_csv(path, usecols=["id", "amount"])` cuts memory use a lot on wide files.
