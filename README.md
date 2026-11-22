# ApexPay Global Database Architecture & Distributed Systems Portfolio

This repository contains the complete enterprise database engineering design, 
query optimization plans, transactional concurrency specifications, NoSQL models, 
and distributed cloud topologies for the ApexPay financial technology platform.

## Architecture Highlights
- Fully normalized relational core (BCNF) supporting strict double-entry ledger bookkeeping.
- Optimized query access paths cutting execution times by over 99%.
- ACID-compliant transaction models featuring deterministic deadlock avoidance.
- Polyglot persistence stack combining Document, Key-Value, and Graph models.
- Distributed, horizontally sharded architecture based on the Google Cloud Spanner engine.

## Repository Directory Index
- /01_database_design: Relational schemas, integrity rules, and normalization steps.
- /02_query_optimization: Unindexed baseline plans vs. optimized index plans.
- /03_transactions_concurrency: Concurrency control, MVCC analysis, and rollback designs.
- /04_nosql_advanced_models: MongoDB audit logs, Redis session caches, and Neo4j fraud graphs.
- /05_distributed_cloud_database: Multi-region failover, 2PC cross-shard transfers, and CAP analysis.
- /evidence_and_artifacts: Query execution plans, trace reports, and architecture diagrams.
- /final_documentation: Executive summaries, reflections, and references.

## System Invariants
- Available balances cannot drop below approved overdraft limits.
- Historical transaction records cannot be modified or deleted.
- Data writes prioritize consistency over availability during network partitions (CP model).# ApexPay_Global
