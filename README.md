# Pandas-perf-comp
A performance comparison between unoptimized Pandas code and a vectorized version. The comparison code and cells can be viewed in the notebook "cudf_pandas_comparison".

The inspiration and basic template for this code was a Sentdex video - https://youtu.be/OnYGtKQT-rU?si=aie4iMvQAFbqDddA

The dataset I am using was made by myself, it has 9 columns and 2 * 10^7 rows and is around 1.5GB big.

Comparison details:

                          Unoptimized              |        Vectorized    | Speedup
    Op 1 (Groupby)          4 min 2 seconds        | 2.24 secs            |  119x
    Op 2 (Group w/ sorting) 19 min 43 secs         | 13.5 secs            |  87x

