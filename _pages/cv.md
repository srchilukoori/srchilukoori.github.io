---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Summary
======
* 14 years setting technical direction for data platforms — defining architectures, evaluating approaches, and replacing fragmented systems with unified ones.
* Deep problem solver shipping production systems in Python, Scala, and Rust — diagnosing root causes and choosing the right tool, even when unconventional.
* Raises the engineering bar beyond individual contributions — building frameworks teams adopt as standards, AI tools that multiply review capacity, and mentoring across levels.
* Active open-source contributor to Apache Airflow and MLCommons Croissant.

Technical Skills
======
* **Languages:** Python, Scala, Rust, SQL
* **Data Platforms:** Spark, Snowflake, Hive, Presto, Trino, EMR
* **Table Formats:** Iceberg, Delta, Parquet, ORC
* **Databases:** Oracle, MySQL
* **Orchestration:** Airflow, Cron
* **Development Tools:** Git, Docker, Jupyter, EMR Studio
* **Cloud Services:** AWS (EMR, S3, Lambda, Step Functions, Secrets Manager)

Experience
======

### Meta Platforms Inc — Menlo Park, CA

**Staff Data Engineer - Ads ML Infra & Governance** (Jul 2025 – Present)

*500+ Ads ML model types and 45K features lacked unified governance — model health, feature impact, and deprecation candidates were tracked through duplicated, inconsistent queries.*

* Aligned geographically distributed technical leads to standardize MTLC metric definitions, consolidating duplicated query logic into a single source of truth
* 90% fewer leadership escalations; root cause analysis reduced from hours to minutes through metric standardization and lineage tracing
* Developed a code review skill after AI-assisted development drove a 3x surge in PR volume — validates coding principles, warehouse entity diagrams, privacy lineage policies, and SQL correctness; adopted by the team for self-review, cutting review time 50%
* Partnered with XFNs to architect a fault-tolerant oncall triage agent for cascading pipeline failures from capacity crunches; the agent identifies upstream dependency blockers, triggers backfills, and generates schema migration PRs, reducing manual investigation time
* Scaled the feature importance pipeline from ad-hoc to weekly execution across 45K features and 500 model types, with S3-backed fault tolerance — enabled data science to identify low-impact feature cohorts for deprecation
* Mentored engineers across levels and functions — from coaching on work visibility during a manager transition, to building a first technical roadmap, to cross-skilling a network engineer into data engineering

**Staff Data Engineer - Marketing Decision Science** (Jan 2024 – Jul 2025)

*Campaign spend across 50+ media channels had no unified platform — ingestion was manual, vendor data lagged weeks, and accuracy was unvalidated.*

* Designed and built the Media Warehouse, a unified data platform tracking multi-hundred-million-dollar marketing spend across 50+ online and offline channels covering US and Europe
* Evaluated vendor data delivery via SFTP, identified ±30% accuracy gaps, and advocated for direct API ingestion — reduced data onboarding from 6 weeks to days
* Built an ingestion module pulling campaign spend from Google Ads, DCM, Reddit, TikTok, and Snapchat, normalizing spend, impression, and conversion metrics into a common schema
* Codified data quality checks in Python and advised agency partners on implementing validation standards to catch precision and format errors before delivery
* Reduced campaign spend data discrepancy from ±30% to within 5% of planned budgets, enabling the central data science team to launch media-mix modeling for Instagram campaigns

### LendingClub Bank NA — San Francisco, CA

**Lead Data Engineer, Analytics** (Sep 2021 – Dec 2023)

*Analytics infrastructure faced scaling bottlenecks — manual job scheduling, fragmented data across on-prem lake and Snowflake, and no standardized pipeline framework.*

* Steered the architectural migration from the on-prem data lake to Snowflake, aligning engineering teams on PySpark, external tables, and Iceberg/Delta formats
* Developed a reusable Airflow operator framework replacing Hue schedules, enabling teams to schedule SQL, HQL, Python, and Snowflake jobs through git-reviewed config without writing custom DAGs, and retiring ~80 redundant service accounts as an infosec improvement
* Influenced engineering leadership to transition the credit evaluation pipeline from Spark to Ray Data — Spark executors had been idling during API calls while holding partitioned data for 5M profiles; Ray's 300 concurrent workers and streaming write-back cut compute from 125 EC2 instances and 24 hours to a single instance in 2 hours
* Engineered a distributed compaction service with the platform team — a Scala crawler identified fragmented partitions across 8K+ tables and 5M+ files, persisted state to DynamoDB, while Lambda functions orchestrated concurrent Spark compaction jobs, restoring 4–10x query performance
* Extended the service to detect and rewrite ORC files with an invalid timezone, unblocking Snowflake external table access for data science and ML workloads
* Led pipeline optimization workshops and code reviews for Hive, Spark, PySpark, and Airflow DAGs

**Sr. Data Engineer, Analytics** (Oct 2019 – Aug 2021)

*Marketing and product teams were blocked on manual processes — no self-service data infrastructure, no automated tooling for faster decision cycles.*

* Automated SEM keyword and auction bid management with Python and the Google Ads API, replacing days of manual effort
* Delivered a profitability data mart in Hive and Presto allocating expenses across loan lifecycle stages (leads, marketing, credit review, origination, servicing), revealing $0.5M/year in wasted lead-channel spend on credit-score segments excluded from the lending program
* Built a repeat-borrower identification system in Python serving product, marketing, and credit risk teams

### Earlier Experience

**Sr. Business Intelligence Developer** — LendingClub Bank NA, San Francisco, CA (Jun 2016 – Sep 2019)

**Sr. Business Intelligence Consultant** — EastBay BI Inc., San Jose, CA (Jan 2013 – May 2016)

*Clients: IDT (semiconductors), Cisco Systems (networking), Nexeo Solutions (chemical distribution).*

* Designed star-schema and bridge-table data models for operational reporting across lending operations, semiconductor manufacturing, and enterprise networking
* Created executive dashboards for investment operations, chip development lifecycle, and service revenue tracking
* Led BI platform migrations across multiple environments: Informix-to-Oracle, SAP-to-QlikView, and QlikView server infrastructure scaling

Open Source Contributions
======
* [Apache Airflow](https://github.com/apache/airflow) — Active Contributor (2026 – Present)
* [MLCommons Croissant](https://github.com/mlcommons/croissant) — Active Contributor (2026 – Present)

Affiliations
======
* [Association for Computing Machinery](https://www.acm.org/) — Member (2022 – Present)

Education
======
* M.S. Mechanical Engineering — [University of Utah](https://www.utah.edu/), Salt Lake City (Aug 2009 – Dec 2012)
* B.Tech. Mechanical Engineering — [National Institute of Technology](https://nitsri.ac.in/), Srinagar, J&K, IN (Aug 2005 – Jul 2009)
