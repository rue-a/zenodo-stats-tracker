# Zenodo Stats Tracker

This repository automatically tracks view and download statistics for specific Zenodo records on a monthly basis.

## How it works
- **Script:** `scripts/fetch_stats.py` queries the Zenodo REST API.
- **Automation:** A GitHub Action runs on the 1st of every month.
- **Storage:** Data is appended to `data/stats_history.csv`.

## Setup
1. Add your Record IDs to the `RECORD_IDS` list in `scripts/fetch_stats.py`.
2. Ensure the GitHub Action has "Read and Write" permissions to commit changes back to the repo.
