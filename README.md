# Awesome-Data-Transformation-Platform

## Top Data Transformation Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on SQL-First Transformations, Analytics Engineering, Data Modeling & Pipeline Orchestration*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Transformation**. These tools help analytics engineers and data teams build modular, testable, version-controlled data pipelines that transform raw data into analytics-ready datasets.



**Examples** include dbt Cloud, Coalesce, Dataform, SQLMesh, Prophecy, Matillion Data Productivity Cloud, DataOps.live, WhereScape RED, Altimate AI, Y42, Kestra, Rivery, and Upsolver (the category leaders).



**Open-source emphasis**: Data transformation has a **mature and production-proven open-source ecosystem**. **dbt Core** is the de facto standard for SQL-based transformations, with the largest community and package ecosystem . **SQLMesh** is a next-generation framework under Linux Foundation governance, offering virtual data environments, column-level lineage, and ~9x faster execution than dbt Core . **Dataform Core** provides BigQuery-native transformations with JavaScript templating . **Kestra** delivers declarative, language-agnostic orchestration for data, AI, and infrastructure workflows . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[dbt Cloud](https://www.getdbt.com/)**  

  The managed platform for dbt, the de facto standard for SQL-based data transformation. Provides a cloud IDE, scheduling, CI/CD, observability, and a private package registry . The largest ecosystem and talent pool in analytics engineering .



- **[Coalesce](https://coalesce.io/)**  

  Metadata-driven data transformation platform that blends visual DAG-based development with code-based workflows. Provides column-level lineage, built-in testing and standards, and AI assistants for SQL generation and documentation . Customers report 10x faster pipeline delivery, 75% faster nightly batch processing, and 50%+ compute reclaimed .



- **[Dataform](https://cloud.google.com/dataform)**  

  Google-owned, BigQuery-native transformation tool. Provides SQLX meta-language with JavaScript templating, dependency management, automated data quality testing, and data documentation . Tightly integrated into BigQuery with hermetic compilation and real-time SQL preview .



- **[Prophecy](https://www.prophecy.ai/)**  

  AI-native data pipeline platform. Enables analysts to generate pipelines with natural language, refine visually or in SQL, and run recurring data flows on their cloud data platform . Supports Snowflake, Databricks, and BigQuery fabrics with SQL Shell for ad-hoc queries .



- **[Matillion Data Productivity Cloud](https://www.matillion.com/)**  

  Enterprise ELT and transformation platform with AI-powered Matillion Copilot (Maia). Provides no-code and high-code options (SQL, Python, dbt), native Git integration, and unstructured data connectors. Customers report 60-70% faster pipeline building and up to 80% reduction in maintenance time .



- **[DataOps.live](https://www.dataops.live/)**  

  DataOps Automation Platform (Momentum) that unites CI/CD, observability, governance, and data product delivery. Features AI-ready scoring, Metis Data Engineering AI Agent, and Data Product Lineage .



- **[WhereScape RED](https://www.wherescape.com/)**  

  Data warehouse automation platform with metadata-driven development, scheduler integration, and deployment automation .



- **[Altimate AI](https://www.altimate.ai/)**  

  AI-powered data engineering assistant for dbt. Provides query history, bookmarks, and shared team repositories for SQL queries and dbt models .



- **[Y42](https://www.y42.com/)**  

  Unified data platform with asset-based orchestrator. Natively integrates dbt Core, Airbyte, Fivetran, and Python scripts into a single dependency-aware pipeline .



- **[Kestra Cloud](https://kestra.io/)**  

  Managed version of the open-source Kestra orchestration platform. Provides declarative YAML workflows, language-agnostic execution, and European data sovereignty focus .



- **[Rivery](https://rivery.io/)**  

  Complete SaaS ELT platform for ingestion, transformation, orchestration, and reverse ETL. Provides 200+ pre-built connectors, Python and SQL transformations, and version control with CLI/API .



- **[Upsolver](https://www.upsolver.com/)**  

  Self-serve cloud data ingestion service for high-scale workloads. Provides no-code and low-code options, automatic schema evolution, exactly-once delivery, and Apache Iceberg support .



## Open-Source GitHub Projects



### SQL Transformation Frameworks



- **[dbt Core](https://github.com/dbt-labs/dbt-core)**  

  **The de facto standard for SQL-based data transformation.** Open-source tool that enables analysts to transform data using the same practices as software engineers — modular SQL, version control, testing, and documentation . Models are SELECT statements that dbt compiles into tables and views in the warehouse . **The largest community and package ecosystem in analytics engineering** . **Apache-2.0**.



- **[SQLMesh](https://github.com/SQLMesh/sqlmesh)**  

  **Next-generation data transformation framework under Linux Foundation governance.** Provides **virtual data environments** (isolated dev environments without warehouse costs), **Plan/Apply workflow** like Terraform for impact analysis, **column-level lineage**, **automatic change detection** running only necessary transformations, and **unit testing** . Supports **SQL and Python**, transpiles across **10+ SQL dialects**, and is **backwards compatible with dbt** . **~9x faster execution than dbt Core** . Install: `pip install 'sqlmesh[lsp]'` .



- **[Dataform Core](https://github.com/dataform-co/dataform)**  

  **Open-source meta-language for creating SQL tables and workflows in BigQuery.** Extends SQL with dependency management, automated data quality testing, and data documentation . Uses **SQLX files** with config blocks and JavaScript templating. Compiles **hermetically** — same code produces same SQL every time, with no internet access during compilation . Dataform Core 3.0.0 replaced `dataform.json` with `workflow_settings.yaml` . **Apache-2.0**.



### Orchestration Platforms



- **[Kestra](https://github.com/kestra-io/kestra)**  

  **Open-source, declarative orchestration platform for data, AI, and infrastructure workflows.** Uses **YAML** for workflow definitions — version-controllable and auditable via GitOps . **Language-agnostic** execution for Python, Node.js, R, Go, Shell, and more with hundreds of plugins . **Event-driven and scheduled** automation from a single interface. Designed for **millions of workflows** with high availability and fault tolerance . **Built for European data sovereignty** with air-gapped deployment support . **Apache-2.0**.



### Additional Strong Open-Source Options



- **SQL Transformation**: **dbt Core** (de facto standard, largest ecosystem), **SQLMesh** (virtual environments, 9x faster, Linux Foundation), **Dataform Core** (BigQuery-native, SQLX + JS) .

- **Orchestration**: **Kestra** (declarative YAML, language-agnostic, event-driven), **Meltano** (declarative code-first data integration engine) .

- **Data Integration**: **Airbyte** (350+ connectors), **dbt-coves** (CLI for dbt staging model generation) .



**Frameworks for building custom systems**: Combine **dbt Core** or **SQLMesh** for SQL transformation, **Kestra** for declarative orchestration across languages, **Dataform Core** for BigQuery-native pipelines, and **Meltano** for code-first data integration. Add **PostgreSQL** for state persistence and **Docker** for deployment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Data transformation platforms handle sensitive production data; ensure proper access controls and compliance with data governance policies.

- **Open-source reality**: The open-source ecosystem for data transformation is **mature and production-proven**. **dbt Core** is the de facto standard with the largest community and package ecosystem . **SQLMesh** offers next-generation capabilities including virtual data environments, column-level lineage, and ~9x faster execution, governed by the Linux Foundation . **Dataform Core** provides BigQuery-native transformations with hermetic compilation . **Kestra** delivers declarative, language-agnostic orchestration with European data sovereignty focus . However, **commercial platforms** (dbt Cloud, Coalesce, Matillion, DataOps.live) provide **managed infrastructure, AI-powered development, enterprise governance, and dedicated support** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong analytics engineering capacity.
