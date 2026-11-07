# Silver social-media research dataset

A fixed cleaned snapshot of X and Bluesky ticker-post records. Contains 22,775 rows, including non-tech tickers. No labels have been verified by humans. The adjacent manifest records provenance, checksums, schema and cleaning details.

Identifiers were pseudonymized and contact patterns masked. Free-form text may still identify public posts. This repository excludes the secret salt, identity lookup, account sessions and credentials. Access is restricted to research collaborators.

Read with Python and Polars:

```python
import polars as pl

df = pl.read_parquet("silver_2026-11-07T141914308759Z_5b61e195.parquet")
print(df.shape)
print(df.schema)
```
