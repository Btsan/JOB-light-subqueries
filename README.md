# JOB-light-subqueries
CSV files containing the subqueries for each of the queries in the JOB-light and JOB-light-ranges workloads for the IMDB database.

JOB-light is a workload of 70 queries introduced in [Learned Cardinalities by Kipf et al.](https://github.com/andreaskipf/learnedcardinalities).

JOB-light-ranges is a workload of 1000 queries introduced in [NeuroCard by Yang et al.](https://github.com/neurocard/neurocard) and features more range predicates.

The CSV files have 3 columns: `query`, `parent`, and `cardinality`.
- `query`: is the column containing the subquery.
- `parent`: indicates which query from the JOB-light or JOB-light-ranges workload is the parent of the subquery.
- `cardinality`: contains the cardinality for the subquery, ran on a snapshot of the IMDB database.
