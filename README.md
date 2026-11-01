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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Database Management Systems (DBMS) and Cloud Database Platform market is estimated at **$111B to $135B in 2025** and projected to exceed **$160B by 2026** with a compound annual growth rate (CAGR) of 11–13%. The sector is **moderately concentrated among hyperscale cloud providers and legacy enterprise incumbents** (Microsoft, Google, AWS, Oracle, IBM, SAP), while maintaining specialized fragmentation across real-time distributed SQL and analytics database engines.

## SaaS/Hosted Platforms

| Platform | Company Valuation / Market Cap | Pricing (Starting Tier) | Free Tier Limits | Key Highlights & Trade-offs |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft SQL Server / Azure SQL](https://www.microsoft.com/sql-server)** | ~$3.1 Trillion (Market Cap) | $0.007/hr (~$5.00/mo) for DTU Basic; or $0.52/vCore-hour serverless ($15,123/core for Enterprise on-prem) | Free tier includes 100,000 vCore seconds/month, 32 GB data storage, and 32 GB backup storage (or Express edition: 10 GB DB, 4 cores free) | T-SQL stored procedures with Azure integration. Best for .NET/Windows teams; per-core production licensing scales steeply. |
| **[Google Cloud Spanner](https://cloud.google.com/spanner)** | ~$2.1 Trillion (Alphabet Market Cap) | $0.030 per 100 Processing Units (PUs)/hr (~$0.30/node-hr; regional multi-zone ~$1.17/node-hr) | 90-day free trial instance with 10 GiB storage, max 5 databases, and standard edition features | Globally distributed database with GoogleSQL & PostgreSQL dialects. Best for global consistency; trial capped at 90 days. |
| **[PostgreSQL RDS](https://aws.amazon.com/rds/postgresql/)** | ~$2.0 Trillion (Amazon Market Cap) | $0.017/hr (~$12.41/mo) for db.t3.micro (Single-AZ) | AWS Free Tier: 750 hrs/mo of db.t3.micro + 20 GB storage for 12 months (first year only) | Managed PostgreSQL supporting PL/pgSQL & extensions. Eliminates operational overhead; free tier expires after 12 months. |
| **[Oracle Cloud Database](https://www.oracle.com/)** | ~$350 Billion (Market Cap) | $0.336/ECPU-hr (License Included) or $0.0807/ECPU-hr (BYOL); min 2 ECPUs | Always Free tier: 2 Autonomous Databases (ATP/ADW) with 20 GB storage each | Deep PL/SQL stored procedure integration. Best for Oracle enterprise migrations; idle free instances subject to reclamation. |
| **[MySQL HeatWave](https://www.oracle.com/mysql/)** | ~$350 Billion (Oracle Market Cap) | $0.0366/ECPU-hr for MySQL DB System + HeatWave node fees (~$0.0194/GB-hr) | Always Free tier: 5,000 hours and 550 GB storage for single HeatWave node instance | MySQL with SQL/PSM and analytics acceleration. Free tier restricted to single node and latest version without HA. |
| **[SAP HANA Cloud](https://www.sap.com/products/hana.html)** | ~$260 Billion (Market Cap) | €0.75 per Capacity Unit (CU)/mo (~€0.0010/CU-hr; compute instances sized via CUs) | Free tier: 1 instance with 16 GB memory, 80 GB storage, and 1 vCPU (stops nightly; 30-day trial extendable up to 90 days) | In-memory database with SQLScript stored procedures. Tailored for SAP enterprises; premium consumption pricing. |
| **[IBM Db2 on Cloud](https://www.ibm.com/products/db2)** | ~$215 Billion (Market Cap) | $99/mo for Standard Plan (includes 2 vCPUs, 8 GB RAM, and initial storage) | Lite Plan: Perpetually free with 200 MB data storage and max 5 concurrent connections | Db2 engine with SQL PL stored procedures. Lite tier is sandbox-only; production environments require paid Standard/Enterprise tier. |
| **[Snowflake Stored Procedures](https://www.snowflake.com/)** | ~$55–$75 Billion (Market Cap) | $2.00 per credit for Standard Edition (on-demand compute) | 30-day free trial with $400 in usage credits (no perpetual free tier) | Server-side procedural logic in JavaScript, Python, Java, and Scala. Compute costs accrue per credit execution. |
| **[CockroachDB](https://www.cockroachlabs.com/)** | ~$5 Billion (Valuation) | $0.092–$0.18 per vCPU-hr (Standard tier) or $0.50/GiB additional storage | Free tier (Basic / Serverless): 50 Million Request Units (RUs) and 10 GiB storage free per month | Distributed SQL with PL/pgSQL support (v25+). Ideal for horizontal scale; commercial self-hosting subject to license restrictions. |
| **[SingleStore Helios](https://www.singlestore.com/)** | ~$1.3 Billion (Valuation) | $0.99/hr for Standard Starter Workspace | Free Starter Shared Workspace: 1 GB compressed storage (~4 GB uncompressed data) for evaluation | Distributed SQL and real-time analytics with stored procedures. Free tier runs on shared infrastructure for non-production use. |

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
