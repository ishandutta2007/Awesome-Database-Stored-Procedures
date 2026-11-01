# Awesome-Database-Stored-Procedures

# Awesome-Database-Stored-Procedures
**Top Database Stored Procedures (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Procedural SQL, Server-Side Logic, Cloud-Managed Databases & Self-Hosted Engines*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Database Stored Procedures**. These tools enable developers to encapsulate business logic inside the database—executing procedural code close to the data for performance, security, and reusability—from fully managed cloud databases with proprietary procedural languages to open-source engines that support SQL/PSM, PL/pgSQL, and custom extensions.

**Examples** include Snowflake Stored Procedures, Oracle Cloud Database, Microsoft SQL Server, PostgreSQL RDS, MySQL HeatWave, SAP HANA Cloud, IBM Db2 on Cloud, SingleStore Helios, CockroachDB, and Google Cloud Spanner (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted stored procedures, procedural SQL engines, and open database infrastructure. **Critical note**: The open-source landscape is mature—**PostgreSQL** leads with PL/pgSQL and multi-language support (Python, Perl, Tcl), **MariaDB** adds Oracle PL/SQL compatibility, and **MySQL** provides ubiquitous SQL/PSM support . No open-source engine matches Oracle's PL/SQL depth or SQL Server's T-SQL ecosystem, but for procedural logic, the open-source options are production-proven.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Snowflake Stored Procedures](https://www.snowflake.com/)**
  **Server-side procedural logic** in Snowflake, supporting JavaScript, Python, Java, and Scala. **Pricing**: Credit-based consumption; **no perpetual free tier**, only **30-day trial with $400 in credits** . **Free tier**: Trial only. **Best for**: Snowflake customers wanting procedural logic close to data—**trade-off**: language support varies by runtime; compute costs accrue per execution.

- **[Oracle Cloud Database](https://www.oracle.com/)**
  **PL/SQL stored procedures** with deep enterprise integration. **Pricing**: **Always Free tier** includes **2 Autonomous Databases (ATP/ADW) each with 20 GB storage** . Paid tiers quote-only. **Free tier**: Yes, 2 Autonomous DBs with 20 GB each. **Best for**: enterprises with existing PL/SQL investments wanting cloud migration—**trade-off**: Always Free tier has strict resource limits; idle resources may be reclaimed.

- **[Microsoft SQL Server](https://www.microsoft.com/sql-server)**
  **T-SQL stored procedures** with tight Azure integration. **Pricing**: **Express Edition is free** (10 GB database, 1 socket/4 cores) ; Standard **$3,945/core** (4-core min); Enterprise **$15,123/core** . **Free tier**: Express free with limits. **Best for**: .NET and Windows-centric teams wanting mature T-SQL—**trade-off**: per-core licensing scales steeply for production.

- **[PostgreSQL RDS](https://aws.amazon.com/rds/postgresql/)**
  **Managed PostgreSQL** with PL/pgSQL and extension support. **Pricing**: AWS Free Tier includes **750 hours/month of db.t3.micro** for 12 months plus **20 GB storage** . **Free tier**: Yes, 750 hours/month for 12 months. **Best for**: teams wanting managed PostgreSQL without operational overhead—**trade-off**: free tier expires after 12 months.

- **[MySQL HeatWave](https://www.oracle.com/mysql/)**
  **MySQL with HeatWave acceleration**, supporting SQL/PSM and JavaScript stored programs. **Pricing**: **Always Free tier** includes **MySQL HeatWave with 5,000 hours and 550 GB storage** . **Free tier**: Yes, 5,000 hours/550 GB. **Best for**: teams wanting MySQL with analytics acceleration—**trade-off**: free tier restricts to latest version, single HeatWave node, no HA .

- **[SAP HANA Cloud](https://www.sap.com/products/hana.html)**
  **In-memory database** with SQLScript stored procedures and multi-model support. **Pricing**: **No free version**; **free trial available**; paid starts at **$9.48/year** per Capterra listings . **Free tier**: Trial only. **Best for**: SAP-centric enterprises needing in-memory procedural logic—**trade-off**: no perpetual free tier; premium pricing.

- **[IBM Db2 on Cloud](https://www.ibm.com/products/db2)**
  **Db2 with SQL PL stored procedures**. **Pricing**: **Lite plan free** with **200 MB storage and 5 connections** ; paid **$99/month** for full functions plus **$200 credits** . **Free tier**: Yes, 200 MB. **Best for**: IBM-centric teams wanting Db2 procedural logic—**trade-off**: Lite plan is sandbox-only; production requires paid tier.

- **[SingleStore Helios](https://www.singlestore.com/)**
  **Distributed SQL with stored procedures** and programmability. **Pricing**: **Free Shared Workspace** (evaluation/non-production); paid **Standard from $0.99/hour** . **Free tier**: Yes, free workspace. **Best for**: teams wanting real-time analytics with procedural logic—**trade-off**: free workspace for non-production only.

- **[CockroachDB](https://www.cockroachlabs.com/)**
  **Distributed SQL with PL/pgSQL stored procedures** (v25+). **Pricing**: **Basic free with 10 GB storage and 50M RU/month** ; **Standard from $0.50/vCPU/hour** . **Free tier**: Yes, 10 GB. **Best for**: teams needing distributed SQL with PostgreSQL-compatible procedures—**trade-off**: PL/pgSQL support is newer (v25); license restrictions for commercial self-hosting .

- **[Google Cloud Spanner](https://cloud.google.com/spanner)**
  **Globally distributed database** with stored procedures via GoogleSQL and PostgreSQL dialects. **Pricing**: **Free trial instance for 90 days** with Standard and Enterprise features . **Free tier**: Yes, 90-day trial instance. **Best for**: teams needing global consistency with procedural logic—**trade-off**: trial expires after 90 days; paid instances require upgrade.

## Open-Source GitHub Projects

- **[PostgreSQL](https://github.com/postgres/postgres)**
  **Advanced open-source relational database** (PostgreSQL License) — **the most feature-complete open-source engine for stored procedures**, supporting **PL/pgSQL** plus **Python, Perl, and Tcl** . **Features**: Full SQL standard compliance; rich extension ecosystem (PostGIS, pgvector); MVCC concurrency; JSONB; logical replication; **procedural languages** as first-class extensions. **Tech stack**: C. **Deploy**: Self-hosted or managed (RDS, Cloud SQL, Azure). **Trade-off**: **Higher learning curve than MySQL**; initial configuration requires tuning . **Best for**: teams needing complex procedural logic with multi-language support—the strongest open-source stored procedure engine.

- **[MariaDB](https://github.com/MariaDB/server)**
  **MySQL-compatible database with Oracle PL/SQL support** (GPL v2) — **the most compatible open-source drop-in replacement**, with features MySQL lacks . **Features**: **SQL/PSM stored procedures**; **Oracle PL/SQL compatibility**—run Oracle procedures with minimal changes ; Galera Cluster for multi-master replication; ColumnStore analytics; **stored procedures as a first-class feature** . **Tech stack**: C++. **Deploy**: Self-hosted or managed. **Trade-off**: **Diverging from MySQL**—bidirectional compatibility maintenance costs rise . **Best for**: teams migrating from MySQL or Oracle wanting PL/SQL compatibility—especially those seeking a truly open-source MySQL alternative.

- **[MySQL](https://github.com/mysql/mysql-server)**
  **The world's most deployed open-source database** (GPL v2, dual-licensed) — **the standard for web application stored procedures**. **Features**: **SQL/PSM stored procedures**; massive ecosystem of tools and managed services; Group Replication for HA; MySQL Shell with JavaScript/Python scripting . **Tech stack**: C++. **Deploy**: Self-hosted or managed (RDS, Cloud SQL, Azure). **Trade-off**: **Less SQL-standard compliant than PostgreSQL**; weaker JSON support; Oracle ownership raises community concerns . **Best for**: teams already in the LAMP stack wanting ubiquitous procedural SQL support.

### Additional Strong Open-Source Options

- **SQLite** — Embedded database with limited trigger-based logic (Public Domain). **Note**: **No stored procedures in the traditional sense**—triggers only; not for server-side procedural logic . **Best for**: embedded and mobile applications, not procedural workloads.
- **TiDB** — MySQL-compatible distributed HTAP database (Apache 2.0). **Note**: MySQL protocol compatible; stored procedure support exists but compatibility details differ from MySQL . **Best for**: teams wanting horizontal scaling with MySQL compatibility.

**Frameworks for building custom systems**: Choose **PostgreSQL** for multi-language procedural logic, **MariaDB** for Oracle PL/SQL compatibility, and **MySQL** for ubiquitous SQL/PSM support—each serves a distinct migration or greenfield scenario. **None of these match Oracle's PL/SQL depth or SQL Server's T-SQL ecosystem**, but for open-source procedural logic, the options are production-proven.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Database platforms handling stored procedures must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls for procedural code.
- **The "proprietary procedural language" vs. "SQL/PSM" vs. "PL/pgSQL multi-language" distinction is critical.** **Oracle (PL/SQL) and SQL Server (T-SQL)** have **proprietary procedural languages** with deep enterprise ecosystems . **MySQL, MariaDB, and SingleStore** use **SQL/PSM**—the standard procedural SQL . **PostgreSQL** uses **PL/pgSQL plus Python, Perl, and Tcl**—the most multi-language support . **Choose based on whether you need Oracle compatibility, standard SQL/PSM, or multi-language flexibility.**
- **Snowflake and SAP HANA Cloud have no perpetual free tier.** Snowflake offers only a **30-day trial with $400 credits** ; SAP HANA Cloud offers **trial only** . **Do not plan a free Snowflake or HANA evaluation beyond trial.**
- **Oracle Always Free tier is genuinely permanent**—**2 Autonomous Databases with 20 GB each** . **The trade-off**: idle resources may be reclaimed with short notice .
- **MySQL HeatWave Always Free is the most generous database free tier**—**5,000 hours and 550 GB storage** . **The trade-off**: latest version only, single HeatWave node, no HA, no point-in-time recovery .
- **CockroachDB's PL/pgSQL support arrived in v25**—it is newer than PostgreSQL's decades-old PL/pgSQL . **For critical procedural workloads, PostgreSQL remains the safer choice.**
- **MariaDB's Oracle PL/SQL compatibility is a genuine migration enabler**—it can run Oracle stored procedures with minimal changes . **For Oracle-to-open-source migrations, it is the strongest option.**
- **Pricing opacity varies.** Snowflake, Oracle, SQL Server, RDS, HeatWave, SAP HANA, Db2, SingleStore, CockroachDB, and Spanner all publish some pricing or free tiers, but enterprise tiers require sales contact. **Validate with direct vendor conversations against your workload profile.**
- Self-hosted open-source solutions require proper infrastructure (compute, storage, backup), security hardening, and ongoing maintenance. **Stored procedures execute business-critical logic**—ensure your deployment meets your organization's reliability and security requirements before migrating production workloads.

---

**Made for database administrators, backend developers, and organizations building transparent procedural logic solutions.**
Let's make Database Stored Procedures more open, data-driven, and logic-friendly.
