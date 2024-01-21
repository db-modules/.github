## 🌱 The Foundation
> “What I cannot create, I do not understand” - Richard Feynman

<details>
<summary>Read More</summary>

#### Core Database Components
- [tiny-yacc-parser](https://github.com/dbminions/tiny-yacc-sql-parser): YACC, SQL `Parser`
- [tiny-sql-rewriter](https://github.com/dbminions/tiny-sql-rewriter): SQL `rewriter`, analyser
- [tiny-binder](https://github.com/dbminions/tiny_binder): `Binder`, Catalog, Type Coercion, Function Overloading
- [tiny-dataframe](https://github.com/dbminions/tiny_dataframe): `RBO`, `Execution Engine`, `Push-based Execution`, Runtime, Visitor, Parquet, Arrow
- [tiny-rule-based-optimizer](https://github.com/dbminions/tiny-planner): Parser, `Binder`, Catalog, RBO, `Execution Engine`, `Push Based Execution`
- [tiny-ssi-txn](https://github.com/dbminions/tiny-txn): Snapshot Isolation Level, Serializable `Transactions`
- [lsm tree](https://github.com/dbminions/lsm-tree): `Storage Engine`, Memtable, WAL
- [tiny-java-db](https://github.com/dbminions/tiny-db): `Volcano Model`, Query Optimizer, `Binder`, `Secondary Index`

```markdown
┌───────┐  ┌───────┐  ┌───────┐
│       │  │       │  │       │
│Parse  ├─►│Rewrite├─►│Binder ├──┐   ┌───────┐  ┌───────┐  ┌──────┐    ┌───────┐   ┌───────┐
│       │  │       │  │       │  │   │ RBO   │  │       │  │      │    │ Txn   │   │ Col   │
└───────┘  └───────┘  └───────┘  ├──►│  +    ├─►│ Exec  ├─►│Run   ├───►│  +    |──►| LSM   │
                                 │   │ CBO   │  │Engine │  │time  │    │ WAL   │   │       │
                      ┌───────┐  │   └───────┘  └───────┘  └──────┘    └───────┘   └───────┘
                      │       │  │
                      │Data   ├──┘
                      │Frame  │
                      └───────┘
```

#### Misc Database Components
- [embedded server](https://github.com/dbminions/tiny-embedded-server): `Sockets`
- [workerpool](https://github.com/dbminions/workerpool): `job queue`, `worker pool`
- [memorypool](https://github.com/dbminions/tiny_mpool): `memory management`, `gc lang`
- [lotsaa](https://github.com/dbminions/lotsaa): `benchmark`, `concurrent access`
- [tiny-compiler](https://github.com/dbminions/tiny-compiler): Covers examples for `AST`, ANTLR, and `Visitor` Pattern
- [tiny-dependency-injection](https://github.com/dbminions/tiny-di-framework): `Dependency Injection` Framework

#### Misc Distributed Systems
- [leader election](https://github.com/dbminions/distributed_leader_election): `Layered BFS`, `Flood Max`
- [network topology optimizer](https://github.com/dbminions/network_topology_optimizer): `Heuristics`, `Topology`

</details>

## 🌿 The Plant

> “A complex system that works is invariably found to have evolved from a simple system that worked...” - John Gall

<details>
<summary>Read More</summary>

#### Database Shrunk
- [matrixorigin-lite](https://github.com/dbminions/colexec-db): Vectorized `Execution Engine`, Push based execution model

#### Small Database [Read]
- [HaloDB](https://github.com/dbminions/HaloDB): InMemory, KV, `Log Structure`, Bitcask
- [OHC](https://github.com/dbminions/ohc): Cache, `OffHeap`, GC, Big Cache
- [LevelDB](https://github.com/dbminions/leveldb): Embedded `LSM` Tree
- [StormDB](https://github.com/dbminions/stormdb): Embedded DB similar to HaloDB

#### Lite Database [TODO]
- [cbo](https://github.com/dbminions/optd): Cost based optimizer
- [risingwave-lite](https://github.com/risinglightdb/risinglight): Streaming database
- [TinySQL](https://github.com/dbminions/tinysql): TiDB
- [TinyKV](https://github.com/talent-plan/tinykv): TiKV

#### Small Database [TODO]
- [RoseDB](https://github.com/dbminions/rosedb): Bitcask
- [LotusDB](https://github.com/dbminions/lotusdb): LSM
- [LotusSearch](https://github.com/dbminions/lotusearch): Search
- [Wal](https://github.com/dbminions/wal): WAL
- [DiskHash](https://github.com/dbminions/diskhash): HashMap, WAL

#### Misc Shrunk
- [geo-spark-lite](https://github.com/dbminions/spatial-spark-rdd): `Spark RDD`, `Apache Sedona`, `Spatial Indexing`

</details>

## 🌳 The Tree
> “You don't have to see the whole staircase, just take the first step.”  - Dr. Martin Luther King, Jr.

<details>
<summary>Read More</summary>
  
#### Mature Databases [TODO]
- [Datafusion](https://github.com/apache/arrow-datafusion): tiny neat query engine
- [CockroachDB](https://github.com/cockroachdb/cockroach): well documented, co-exec, has logical/physical optimizer, exec engine
- [Prometheus](https://github.com/dbminions/prometheus): PromQL, TSDB
- [Presto](https://github.com/prestodb/presto): RBO, CBO

#### Misc [Read]
- [Go-YCSB](https://github.com/dbminions/go-ycsb): KV Benchmark, `YCSB`

</details>

## 💧 The Resources
> "It is not that I'm so smart. But I stay with the questions much longer." - Albert Einstein

<details>
<summary>Read More</summary>

#### Books in Pipeline [Reading]
- [100 Go Mistakes and How to Avoid Them](https://a.co/d/7EAXgLq) - Great for understanding common mistakes in `go`.
- [Querify Labs Blog](https://www.querifylabs.com/blog) - Good blog on optimizers.
- [Patterns of Distributed Systems](https://martinfowler.com/articles/patterns-of-distributed-systems/) - `Spanner` 2PC etc.

#### Books on DB [Read]
- [Database Design and Implementation](https://a.co/d/9cJnBev) -  Great for understanding embedded Java databases like Apache `Derby`
- [How Query Engine Works: An Introductory Guide](https://a.co/d/0tnFBHx) - Great for understanding Query Engine like Arrow `Datafusion`
- [Algorithms and Data Structures for Massive Datasets](https://a.co/d/j4aYee9) - BF, `Count-Min` Sketch, HyperLogLog, Reservoir `Sampling`.

#### Database Papers [Read]
- [Google Spanner Paper](https://static.googleusercontent.com/media/research.google.com/en//archive/spanner-osdi2012.pdf) - Distributed `Strict Serializable Transaction` using True Time
- [A method for implementing Lock-Free shared Data Structures](https://dl.acm.org/doi/pdf/10.1145/165231.165265) - Coordination Technique, Caching Algo

#### Misc Papers [Read]
- [Elkan's Kmeans](https://cdn.aaai.org/ICML/2003/ICML03-022.pdf) - Fast `Kmeans` Algorithm using Triangle Inequality Property

</details>

## 👨‍🌾 Cultivating Knowledge
> "If you can't explain it simply, you don't understand it well enough." - Albert Einstein

<details>
<summary>Read More</summary>

#### Database
- [Copy Ahead Segment Ring](https://utd-ir.tdl.org/server/api/core/bitstreams/bca5d1fb-7b45-403c-b435-4d965d387367/content) - New Memtable Design, Evolution of Database Systems
- [TinyDB](https://www.youtube.com/playlist?list=PLVd_ZXv73U8jqQHvW_R5oQF8qo8SHv3Re) - Tiny Database written in Java
- [Method for Implementing lock-free shared data structure](https://www.youtube.com/watch?v=MK1ZqqW-9gM) - Coordination Technique, Large Objects

#### Misc
- [Tiny Compiler](https://medium.com/javarevisited/build-a-tiny-compiler-in-java-662f67a1ce85) - Tiny Compiler written in Java
- [Using spark for spatial data management](https://medium.com/sys-base/spatial-partitioned-rdd-using-kd-tree-in-spark-102e0b53564b) - Spark RDD, KD Tree
- [Design Patterns](https://medium.com/sde-base/design-pattern-in-java-bafd91a5d24e) - Design Pattern from GoF.

</details>


## 🥭 The Fruit
> "It always seems impossible until it's done." - Nelson Mandela

<details>
<summary>Read More</summary>
  
#### Database commits
- [MaxtrixOrigin](https://github.com/matrixorigin/matrixone/commits?author=arjunsk)
- [Vector Index Paper](): Pending
- [Memtable Paper](): Pending

</details>
