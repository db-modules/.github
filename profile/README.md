## 🌱 The Foundation
> “What I cannot create, I do not understand” - Richard Feynman

<details>
<summary>Read More</summary>

#### Core Database Components
- [tiny-yacc-parser](https://github.com/dborchard/tiny-yacc-sql-parser): YACC, SQL `Parser`
- [tiny-sql-rewriter](https://github.com/dborchard/tiny-sql-rewriter): SQL `rewriter`, analyser
- [tiny-binder](https://github.com/dborchard/tiny_binder): `Binder`, Catalog, Type Coercion, Function Overloading
- [tiny-dataframe](https://github.com/dborchard/tiny_dataframe): `RBO`, `Execution Engine`, `Push-based Execution`, Runtime, Visitor, Parquet, Arrow
- [tiny-rule-based-optimizer](https://github.com/dborchard/tiny-planner): Parser, `Binder`, Catalog, RBO, `Execution Engine`, `Push Based Execution`
- [joins](https://github.com/dborchard/joins_impl): Join using Spark Execution Engine. `Grace Hash Join`, `Sort Merge Join`, `Nested Join`
- [tiny-ssi-txn](https://github.com/dborchard/tiny-txn): Snapshot Isolation Level, Serializable `Transactions`
- [lsm tree](https://github.com/dborchard/lsm-tree): `Storage Engine`, Memtable, WAL
- [col-fs](https://github.com/dborchard/col-lsm): Columnar/Row Format, `File Storage`, S3
- [tiny-java-db](https://github.com/dborchard/tiny-db): `Volcano Model`, Query Optimizer, `Binder`, `Secondary Index`

```markdown
┌───────┐  ┌───────┐  ┌───────┐
│       │  │       │  │       │
│Parse  ├─►│Rewrite├─►│Binder ├──┐   ┌───────┐  ┌───────┐  ┌──────┐    ┌───────┐   ┌───────┐
│       │  │       │  │       │  │   │ RBO   │  │       │  │      │    │ Txn   │   │ Col   │
└───────┘  └───────┘  └───────┘  ├──►│  +    ├─►│ Exec  ├─►│Run   ├───►│  +    |──►| LSM   │
                                 │   │ CBO   │  │Engine │  │time  │    │ WAL   │   │       │
                      ┌───────┐  │   └───────┘  └───────┘  └──────┘    └───────┘   └───────┘
                      │Data   │  │
                      │Frame  ├──┘
                      │Builder│
                      └───────┘
```

#### Misc Database Components
- [workerpool](https://github.com/dborchard/workerpool): `job queue`, `worker pool`
- [memorypool](https://github.com/dborchard/tiny_mpool): `memory management`, `gc lang`
- [lotsaa](https://github.com/dborchard/lotsaa): `benchmark`, `concurrent access`
- [tiny-compiler](https://github.com/dborchard/tiny-compiler): Covers examples for `AST`, ANTLR, and `Visitor` Pattern
- [tiny-dependency-injection](https://github.com/dborchard/tiny-di-framework): `Dependency Injection` Framework

</details>

## 🌿 The Plant

> “A complex system that works is invariably found to have evolved from a simple system that worked...” - John Gall

<details>
<summary>Read More</summary>

#### Core Modules [Being Shrunk]
- [MatrixOrigin Join Modules](https://github.com/dborchard/mo_join): Optimizer Runtime Filter, ColExec for SEMI, INNER, LEFT, RIGHT, INDEX, SINGLE joins


#### Database Shrunk [By me]
- [matrixorigin-lite](https://github.com/dborchard/colexec-db): Vectorized `Execution Engine`, Push based execution model
- [prometheus-lite](https://github.com/dborchard/prometheus_lite): Parser, PromQL, `TSDB`
- [crdb-lite](https://github.com/dborchard/tiny_crdb): RBO, CBO, exec engine, type coercion
- tidb-lite: RBO, CBO, exec engine, parser

#### Planning to Shrink
- [PranaDB](https://github.com/cashapp/pranadb): Go
- [M3DB](https://github.com/m3db/m3): Go
- [RadonDB](https://github.com/radondb/radon?tab=readme-ov-file): Go
- [LinDB](https://github.com/lindb/lindb): Go

#### Educational Database [TODO]
- [risingwave-lite](https://github.com/risinglightdb/risinglight): Streaming database
- [datafusion-cbo](https://github.com/dborchard/optd): Cost based optimizer
- [TinySQL](https://github.com/dborchard/tinysql): TiDB
- [TinyKV](https://github.com/talent-plan/tinykv): TiKV
- [BusTub](https://github.com/cmu-db/bustub): CMU

#### Hobby Database [TODO]
- [RoseDB](https://github.com/dborchard/rosedb): Bitcask
- [LotusDB](https://github.com/dborchard/lotusdb): LSM
- [LotusSearch](https://github.com/dborchard/lotusearch): Search
- [Wal](https://github.com/dborchard/wal): WAL
- [DiskHash](https://github.com/dborchard/diskhash): HashMap, WAL

</details>

## 🌳 The Tree
> "The best time to plant a tree was 20 years ago. The second best time is now." - Chinese Proverb

<details>
<summary>Read More</summary>

#### Mature Databases [Read]
- [MatrixOrigin](https://github.com/matrixorigin/matrixone): Go, Vectorized Execution, Parser, Push based
- [Prometheus](https://github.com/dborchard/prometheus): TSDB, PromQL, Loki
- [CockroachDB](https://github.com/cockroachdb/cockroach): Go, RBO, CBO, exec engine
- [TiDB](https://github.com/pingcap/tidb): RBO, CBO, exec engine, Go/Rust


#### Small Codebase Database [Read]
- [HaloDB](https://github.com/dborchard/HaloDB): InMemory, KV, `Log Structure`, Bitcask
- [OHC](https://github.com/dborchard/ohc): Cache, `OffHeap`, GC, Big Cache
- [LevelDB](https://github.com/dborchard/leveldb): Embedded `LSM` Tree
- [StormDB](https://github.com/dborchard/stormdb): Embedded DB similar to HaloDB
- [FrostDB](https://github.com/polarsignals/frostdb): `Push Based Exec`, Arrow, Parquet, `RBO`, Parser, `LSM`

#### Mature Database not written in Go [TODO]
- [Datafusion](https://github.com/apache/arrow-datafusion): Rust, query engine
- [Presto](https://github.com/prestodb/presto): Java, RBO, CBO
- [DuckDB](https://github.com/duckdb/duckdb): C++

#### Misc [Read]
- [Go-YCSB](https://github.com/dborchard/go-ycsb): KV Benchmark, `YCSB`

</details>

## 💧 The Resources
> "You don't understand anything until you learn it more than one way." – Marvin Minsky

<details>
<summary>Read More</summary>

#### Books in Pipeline [Reading]
- [Querify Labs Blog](https://www.querifylabs.com/blog) - Good blog on optimizers.
- [Designing Data-Intensive Applications](https://a.co/d/hwmSC1o)

#### Books on DB Introduction [Read]
- [Database Design and Implementation](https://a.co/d/9cJnBev) -  Great for understanding embedded Java databases like Apache `Derby`
- [How Query Engine Works: An Introductory Guide](https://a.co/d/0tnFBHx) - Great for understanding Query Engine like Arrow `Datafusion`

#### Books on DB Introduction [TODO]
- [Build Your Own Database From Scratch](https://build-your-own.org/database/)
- [Database Internals](https://www.databass.dev/)

#### Database Papers [Read]
- [Awesome DB Papers](https://github.com/dborchard/awesome-db-papers)

</details>

## 👨‍🌾 Cultivating Knowledge
> "If you can't explain it simply, you don't understand it well enough." - Albert Einstein

<details>
<summary>Read More</summary>

#### Database
- [Copy Ahead Segment Ring](https://utd-ir.tdl.org/server/api/core/bitstreams/bca5d1fb-7b45-403c-b435-4d965d387367/content) - New Memtable Design, Evolution of Database Systems
- [TinyDB](https://www.youtube.com/playlist?list=PLVd_ZXv73U8jqQHvW_R5oQF8qo8SHv3Re) - Tiny Database written in Java

#### Misc
- [Tiny Compiler](https://medium.com/javarevisited/build-a-tiny-compiler-in-java-662f67a1ce85) - Tiny Compiler written in Java
- [Design Patterns](https://medium.com/sde-base/design-pattern-in-java-bafd91a5d24e) - Design Pattern from GoF.

</details>


## 🥭 The Fruit
> "It always seems impossible until it's done." - Nelson Mandela

<details>

<summary>Read More</summary>
  
#### Database Work
- [MaxtrixOrigin](https://github.com/matrixorigin/matrixone/commits?author=arjunsk)
- [CometKV](https://github.com/dborchard/cometkv) : WIP, Comparing different memtables

#### Published Materials
- [Vector Index Paper](): Pending
- [Memtable Paper](): Pending

</details>

![](https://komarev.com/ghpvc/?username=dborchard)
