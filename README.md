# Graph Database Benchmark

A comparison of Neo4j, FalkorDB, and Memgraph on a graph derived from product-review data. The study examines ingestion, query execution, concurrency, memory, and startup behavior.

[Read the benchmark on AIMultiple](https://aimultiple.com/graph-databases).

The dataset connects reviews, products, reviewers, brands, features, and categories. Shared query templates cover point lookups, traversals, aggregations, filtering, and scans. Parameterized repetitions capture variation across both popular and less frequent entities.

The benchmark also changes ingestion batch size, increases the number of concurrent clients, and examines mixed read/write workloads. Index tests compare the same query patterns with different indexing conditions.

Each database is evaluated on a single node. The article documents its versions, memory configuration, warmup procedure, and measurement method. Distributed deployments, recovery behavior, and other workload shapes fall outside this comparison. The published results explain which query types account for the observed differences between the tested engines.

The benchmark implementation was developed for AIMultiple and belongs to AIMultiple. This repository is a documentation summary. Source code and benchmark datasets are not distributed here.
