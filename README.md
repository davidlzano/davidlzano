# David A. Lozano Rodríguez

**Data & Business Intelligence Analyst** · Medellín, Colombia

I work on the part of data that almost nobody sees: the integration, modeling and automation that make a dashboard mean something. I started in quality and moved into data full time, and that path shapes how I work — I understand why data arrives dirty, who types it in, and which decision depends on it.

Today I build Python ETL pipelines against transactional-system APIs, model historical data with versioning in SQL Server, develop internal data-capture applications, and design engines that generate operational plans under real constraints.

---

## Projects

All four are demo reimplementations of systems I put into production. Original code, synthetic data, runnable with two commands.

### [Inventory Transfer Optimization Engine](https://github.com/davidlzano/motor-traslados-inventario)

Generates the daily inventory redistribution plan for a store network: what to move, from where, to where, and how much. It solves a variant of the transportation problem with a three-stage prioritized heuristic, respecting product compatibility, each location's dynamic capacity, and freight economics.

In production it covers about 470 stores and replaced a manual exercise that took one week per month.

`Python` · `SQLite` · `pandas`

### [Fault-Tolerant ETL Pipeline](https://github.com/davidlzano/pipeline-etl-tolerante-fallos)

Daily integration from an API into a data warehouse. Self-recovering rolling window, retries with increasing backoff, distinct handling of transient and permanent errors, and row-hash incremental loading that discards whatever did not change.

The simulated API deliberately fails 35% of the time, so fault tolerance can be seen operating instead of just read about.

`Python` · `SQLite` · `pandas`

### [Shop-Floor Data Capture App](https://github.com/davidlzano/app-captura-planta)

Web form for hourly production logging from a phone on the factory floor. The operator enters the machine counter reading and the system derives the production, which removes the error of subtracting in your head every hour. Catalogs that reload without restarting the service, and server-side validation.

`Python` · `Flask` · `SQLite`

### [Versioned Production Schedule History](https://github.com/davidlzano/historico-programacion-planta)

Turns daily backups of a hand-edited Excel file into a database with a queryable timeline. It maps by header name because columns move between files, stores only the changes instead of full snapshots, and tells an unreadable sheet apart from a deleted row.

In production it covers 22 work centers and made it possible to recover from a real data loss.

`Python` · `openpyxl`

---

## Tools

- **Data:** SQL Server · SQL · ETL processes · dimensional modeling · master data (MDM)
- **Python:** pandas · NumPy · Flask · API consumption · automation
- **BI:** Power BI · DAX · advanced Excel (Power Query, Power Pivot, VBA)

---

## Contact

Open to opportunities as a Data or BI Analyst, **remote or hybrid**.

[LinkedIn](https://www.linkedin.com/in/david-a-lozano-rodríguez-7b2a62261) · davidlzano19@gmail.com
