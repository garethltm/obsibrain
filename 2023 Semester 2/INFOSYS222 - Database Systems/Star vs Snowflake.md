|[[Star Schema]]|[[Snowflake Schema]]|
|---|---|
|Typically adding DATA into the [[Facts]] area|Can add into different areas|
|[[Dimension]] is usually static|Not as static|
|Queries efficient|Data loading efficient|
|Storage space not good|Storage space good|

- If you’re always adding/changing items (like customer, etc.), its better to use a [[Snowflake Schema]] approach

Think about whether if you run queries most of the time where you are concerned with the storage space