# Pandas-perf-comp
A performance comparison between unoptimized Pandas code and a vectorized version. The comparison code and cells can be viewed in the notebook "cudf_pandas_comparison".

The dataset I am using was made by myself, it has 9 columns and 2 * 10^7 rows and is around 1.5GB big.

Comparison details:

&emsp &emsp &emsp  Unoptimized    |    Vectorized
Operation 1 (Groupby) 4 min 2 seconds | 2.24 secs
Operation 2 (Groupby w/ sorting) 19 min 43 secs | 13.5 secs

