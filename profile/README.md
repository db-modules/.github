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
> "It is not that I'm so smart. But I stay with the questions much longer." - Albert Einstein

<details>
<summary>Read More</summary>

#### Papers
- [Spanner](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf) - Distributed `Strict Serializable Transaction` using True Time
- [Elkan's Kmeans](https://cdn.aaai.org/ICML/2003/ICML03-022.pdf) - Fast `Kmeans` Algorithm using Triangle Inequality Property

#### Books
- [Patterns of Distributed Systems](https://martinfowler.com/articles/patterns-of-distributed-systems/) - `Spanner` 2PC etc.
- [Algorithms and Data Structures for Massive Datasets](https://a.co/d/j4aYee9) - BF, `Count-Min` Sketch, HyperLogLog, Reservoir `Sampling`.
- [Database Design and Implementation](https://a.co/d/9cJnBev) -  Great for understanding embedded Java databases like Apache `Derby`

</details>

## 💻 Real-world Database Systems
> "It always seems impossible until it's done." - Nelson Mandela

<details>
<summary>Read More</summary>
  
#### Production Key-Value Stores
- [HaloDB](https://github.com/db-modules/HaloDB): InMemory, KV, `Log Structure`, Bitcask
- [OHC](https://github.com/db-modules/ohc): Cache, `OffHeap`, GC, Big Cache
- [LevelDB](https://github.com/db-modules/leveldb): `LSM` Tree
- [StormDB](https://github.com/db-modules/stormdb): Similar to HaloDB
- [Go-YCSB](https://github.com/db-modules/go-ycsb): KV Benchmark, `YCSB`

#### Production Distributed Databases (Planning to Learn)
- [Pinot](https://github.com/apache/pinot)
- [Presto](https://github.com/prestodb/presto)
- [Drill](https://github.com/apache/drill)
- [Druid](https://github.com/apache/druid)

</details>

## ✍ My attempts to teach
> "If you can't explain it simply, you don't understand it well enough." - Albert Einstein

<details>
<summary>Read More</summary>

#### Technical works
- [Copy Ahead Segment Ring](https://utd-ir.tdl.org/server/api/core/bitstreams/bca5d1fb-7b45-403c-b435-4d965d387367/content) - New Memtable Design, Evolution of Database Systems
- [Method for Implementing lock-free shared data structure](https://www.youtube.com/watch?v=MK1ZqqW-9gM) - Coordination Technique, Large Objects
- [TinyDB](https://www.youtube.com/playlist?list=PLVd_ZXv73U8jqQHvW_R5oQF8qo8SHv3Re) - Tiny Database written in Java
- [Tiny Compiler](https://medium.com/javarevisited/build-a-tiny-compiler-in-java-662f67a1ce85) - Tiny Compiler written in Java
- [Using spark for spatial data management](https://medium.com/sys-base/spatial-partitioned-rdd-using-kd-tree-in-spark-102e0b53564b) - Spark RDD, KD Tree
- [Design Patterns](https://medium.com/sde-base/design-pattern-in-java-bafd91a5d24e) - Design Pattern from GoF.

</details>
