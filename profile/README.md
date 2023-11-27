## 📎 Tiny Database Modules
> “You don't have to see the whole staircase, just take the first step.”  - Dr. Martin Luther King, Jr.

<details>
<summary>Read More</summary>
  
#### Individual Database Components
- [yacc parser](https://github.com/db-modules/tiny-yacc-sql-parser): `YACC`, SQL Parser
- [tiny-planner](https://github.com/db-modules/tiny-planner): LogicalPlan `Builder`, Logical Plan Rule Based `Optimizer`, `Execution` Engine
- [tiny-exec-engine](https://github.com/db-modules/colexec-db) : Vectorized `Execution Engine`
- [serializable snapshot isolation](https://github.com/db-modules/serialized-snapshot-isolation): `Isolation Level`, Transactions
- [lsm tree](https://github.com/db-modules/lsm-tree): `Storage Engine`, Memtable, WAL
- [tiny-java-db](https://github.com/db-modules/tiny-db): `Volcano Model`, Query Optimizer

#### Misc Database Components
- [embedded server](https://github.com/db-modules/tiny-embedded-server): `Sockets`
- [workerpool](https://github.com/db-modules/workerpool): `job queue`, `worker pool`
- [lotsaa](https://github.com/db-modules/lotsaa): `benchmark`, `concurrent access`

#### Simple Distributed Systems
- [leader election](https://github.com/db-modules/distributed_leader_election): `Layered BFS`, `Flood Max`
- [network topology optimizer](https://github.com/db-modules/network_topology_optimizer): `Heuristics`, `Topology`
- [geo-spark-lite](https://github.com/db-modules/spatial-spark-rdd): `Spark RDD`, `Apache Sedona`, `Spatial Indexing`

</details>

## 📗 Resources Read

<details>
<summary>Read More</summary>

#### Papers
- [Spanner](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf) - Distributed Transaction using True Time
- [Using the Triangle Inequality to Accelerate K-Means](https://cdn.aaai.org/ICML/2003/ICML03-022.pdf) - Elkan's Kmeans

#### Books
- [Patterns of Distributed Systems](https://martinfowler.com/articles/patterns-of-distributed-systems/) - Good for learning more about Spanner 2PC etc.
- [Algorithms and Data Structures for Massive Datasets](https://www.amazon.com/Algorithms-Data-Structures-Massive-Datasets/dp/1617298034) - Great for learning about new data structures.
- [Database Design and Implementation](https://www.amazon.com/dp/3030338355/) -  Great for understanding embedded Java databases like Apache Derby

</details>

## 💻 Real-world Database Systems
> "It always seems impossible until it's done." - Nelson Mandela

<details>
<summary>Read More</summary>
  
#### Production Databases Learned
- [HaloDB](https://github.com/db-modules/HaloDB): InMemory, KV, Log Based, Bitcask
- [OHC](https://github.com/db-modules/ohc): Cache, OffHeap, GC
- [LevelDB](https://github.com/db-modules/leveldb): LSM Tree
- [StormDB](https://github.com/db-modules/stormdb): Similar to HaloDB
- [Go-YCSB](https://github.com/db-modules/go-ycsb): benchmark, YCSB

</details>
