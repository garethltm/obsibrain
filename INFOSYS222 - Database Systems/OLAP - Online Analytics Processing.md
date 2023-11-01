## [[INFOSYS222 - Database Systems/Database]]
- designed for complex querying & reporting tasks
- [[Analytics]] tasks

## Schema
- Multidimensional model based on:
    - [[Facts]]
    - Dimension
- [[Star Schema]]/[[Snowflake Schema]]
- [[Denormalisation]] - avoid the multiple JOINS
    - Slower in running queries

## SQL
- Running on large datasets - query intensive to generate an output
- Access control is not as important:
    - If mistake you can always load your data again from the [[Data Warehouse]]
- Concurrency control is not as important:
    - You can run sequential/parallel - just accessing information & not updating anything
- Query performance is important:
    - Do indexing, pre-aggregation & caching