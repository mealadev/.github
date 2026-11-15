# Meala (`mealadev`)

**Open-source multi-user flight log database, cross-stack telemetry normalizer, and fleet analytics platform for UAV & autonomous systems teams.**

Meala turns scattered binary flight logs (`.bin`, `.ulg`, `.tlog`, `.bbl`) from ArduPilot, PX4, and INAV into a unified, SQL-queryable Apache Parquet telemetry index—available both as a **self-hosted multi-user server** and a **local-first Jupyter/Python toolkit**.

---

### Core Ecosystem Repositories

| Repository | Description |
| :--- | :--- |
| **[`mealadev/meala`](https://github.com/mealadev/meala)** | Self-hosted Docker Compose platform (`FastAPI` + `PostgreSQL` + `Nginx` multi-log overlay UI) for UAV teams. |
| **[`mealadev/meala-jupyter`](https://github.com/mealadev/meala-jupyter)** | Local-first Jupyter Notebook & Python toolkit using SQLite and Apache Parquet for offline flight forensics. |
| **[`mealadev/.github`](https://github.com/mealadev/.github)** | Organization profile, issue forms, pull request templates, and security policies. |

---

### Key Capabilities

* **Unified Telemetry Schema:** Converts disparate autopilot binary logs into canonical Pandas DataFrames and compressed Apache Parquet files.
* **Instant SQL Filtering:** Query thousands of flights by ambient weather, battery voltage sag, vibration thresholds, EKF failsafes, firmware Git hash, or pilot notes.
* **Multi-Log Comparison:** Overlay up to four heterogeneous logs (e.g., ArduPilot `.bin` vs. PX4 `.ulg`) side-by-side or in synchronized grid mode.
* **Automated Weather Enrichment:** Correlates takeoff coordinates and UTC timestamps against historical meteorological records to uncover environmental hardware failures.

---

### Links & Community

* **Website & Documentation:** [meala.dev](https://meala.dev)
* **Community Q&A & Ideas:** [GitHub Discussions](https://github.com/orgs/mealadev/discussions)
* **Security Disclosures:** `security@meala.dev`
