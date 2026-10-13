# NBA Data Pipeline (Oddsix foundation)

The starting point of [Oddsix](https://oddsix.app), my multi-sport data and prediction platform. This repository
is preserved as it was in early 2026: a data pipeline written by hand, before the project grew into the full
platform with AI-assisted development.

## What it does

- Pulls game logs, player stats, team stats and a player master list from the NBA Stats API with Python
- Cleans and standardizes the raw data (consistent IDs, seasons, column names and types)
- Loads the cleaned data into a relational SQLite database (`database/nba.db`) for analysis

## Structure

| Path | What it is |
|---|---|
| `src/data/` | Scripts that pull each dataset from the NBA Stats API |
| `src/processing/preprocessing_data.ipynb` | Cleaning and standardization |
| `src/processing/load_to_sql.py` | Loads the processed data into the database |
| `database/nba.db` | The resulting SQLite database |
| `docs/project_overview.md` | Progress log: planning, architecture, ingestion, cleaning and the SQL layer |

## Status

Archived. Development continued in the private Oddsix codebase, which now covers five leagues with live updates,
prediction models and a public website at [oddsix.app](https://oddsix.app).
