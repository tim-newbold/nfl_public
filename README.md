# 🏈 NFL ETL Engine (Python + SQL Server)

This repository contains a Python-based ETL engine that pulls NFL data using the [`nfl_data_py`](https://nfl-data-py.readthedocs.io/en/latest/) API and loads it into a local SQL Server database. The data can then be used for dashboards, analysis, or machine learning models.

---

## 📦 Tech Stack

- **Python** (ETL & automation)
- **SQL Server** (local storage and dashboard backend)
- **SQLAlchemy + pyodbc** (database connection)
- **nfl_data_py** (data ingestion from NFL sources)
- **pandas** (data wrangling)

## 📥 Weekly ETL Functions

| Function                          | Description                       | Target Table       |
|----------------------------------|-----------------------------------|--------------------|
| `getnextgenpassing(year, week, engine)`   | Pulls passing NGS stats by week     | `next_gen_passing` |
| `getnextgenrushing(year, week, engine)`   | Pulls rushing NGS stats by week     | `next_gen_rushing` |
| `getnextgenreceiving(year, week, engine)` | Pulls receiving NGS stats by week   | `next_gen_receiving` |
| `getweeklystats(year, week, engine)`      | Weekly player stats                 | `week_stats`       |
| `getplaybyplay(year, week, engine)`       | Full play-by-play data              | `plays`            |
| `getweeklyschedule(year, week, engine)`   | Weekly NFL schedule                 | `schedule_xref`    |

## 🧭 One-Time or Historical Loads

| Function                        | Description                         | Target Table     |
|--------------------------------|-------------------------------------|------------------|
| `getteamxref(engine)`          | NFL team cross-reference info       | `team_xref`      |
| `getplayerroster(year, engine)`| Roster data by season               | `rosters_xref`   |
| `getschedule(year, engine)`    | Full NFL schedule by year           | `schedule_xref`  |

## Power BI Dashboard Examples
- Located in images!
