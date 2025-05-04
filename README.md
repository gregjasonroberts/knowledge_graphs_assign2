# knowledge_graphs_assign2
Repo for 2nd individual assignment

# README

This repository provides an overview of key database and knowledge‑graph technologies, organized into five parts. Each section includes a brief summary and a source link or reference for further reading.

---

## Part 1 – Relation Extraction (RE)

Relation Extraction (RE) focuses on identifying and classifying semantic relationships between entities in text, constructing the edges of a knowledge graph. RE operates at both the mention level (detecting relations within a single sentence) and the global level (aggregating evidence across multiple contexts). Ontology‑driven constraints ensure only valid entity types are linked (e.g., a `PERSON` to an `ORGANIZATION`). Techniques include kernel methods (e.g., syntactic tree kernels achieving ~77.1% F‑score), semi‑supervised bootstrapping, distant supervision, and multitask transfer learning. RE is powerful for building richly connected graphs but faces challenges such as complexity, error propagation, and noisy training data.

**Source:** Kejriwal, Mayank, Craig A. Knoblock, and Pedro Szekely. *Knowledge Graphs: Fundamentals, Techniques, and Applications*. Cambridge, MA: MIT Press, 2021. Chapter 6, Relation Extraction, pp. 125–147. ISBN-13: 978-0262045094

---

## Part 2 – Gel/EdgeDB

Gel (formerly EdgeDB) introduces a graph‑relational data model that structures data as object types connected by explicit links, eliminating the need for traditional JOINs. EdgeQL, its native query language, offers concise hierarchical `SELECT`, `INSERT`, and `UPDATE` operations. The platform includes integrated developer tools—schema browser, data editor, visual query builder, and web‑based REPL—for seamless schema introspection and query prototyping.

**Source:** [EdgeDB is now Gel, and Postgres is the Future](https://www.geldata.com/blog/edgedb-is-now-gel-and-postgres-is-the-future)

---

## Part 3 – TimescaleDB

TimescaleDB extends PostgreSQL for time‑series workloads with hypertables (automatic time‑based partitioning), continuous aggregates (incrementally maintained materialized views), and native compression/tiered storage (up to 95% storage reduction and offloading to Amazon S3). These features optimize ingestion, querying, and analysis of large time‑series datasets.

**Source:** [TimescaleDB – An Introduction to Time Series Databases](https://medium.com/dataengineering-and-algorithms/timescaledb-an-introduction-to-time-series-databases-3438d275e88e)

---

## Part 4 – ParadeDB

ParadeDB builds on PostgreSQL to deliver advanced full‑text search (BM25 via pg_search), hybrid search (pgvector integration), real‑time search/analytics (auto‑synced indexes), faceted search, and high‑performance aggregations—all within the PostgreSQL ecosystem.

**Source:** [Exploring ParadeDB core features and benefits](https://risingwave.com/blog/exploring-paradedb-core-features-and-benefits/)

---

## Part 5 – pgvector

pgvector adds a vector column type to PostgreSQL, supporting high‑dimensional embeddings and multiple similarity operators (Euclidean, cosine, inner product, L1, Hamming, Jaccard). It provides approximate nearest‑neighbor indexes (IVF, HNSW) and integrates with Python frameworks (Django, SQLAlchemy, Psycopg, etc.) via the pgvector‑python library.

**Source:** [Introduction to pgvector: Enhancing PostgreSQL with Vector Data Capabilities](https://medium.com/@interviewbuddies/introduction-to-pgvector-enhancing-postgresql-with-vector-data-capabilities-74844c0398d6)
