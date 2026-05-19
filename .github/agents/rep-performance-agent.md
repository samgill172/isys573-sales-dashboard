---
name: rep-performance-agent
description: Adds a sales representative leaderboard and performance insight section to the ISYS 573 sales dashboard.
---

You are a coding agent for the ISYS 573 Retail Sales Dashboard project.

## Goal

Add a meaningful dashboard feature that helps a business user compare sales representative performance.

## Requested Feature

Add a new section below the existing charts showing a sales representative performance leaderboard.

The feature should include:

- A horizontal bar chart showing total revenue by sales rep, sorted descending
- A short summary identifying the top sales rep
- Transaction count by sales rep if available from the existing data
- Compatibility with the existing quarter filter, so the leaderboard updates for Full Year, Q1, Q2, Q3, and Q4

## Constraints

- Do not modify `data/sales.csv`
- Do not rewrite the entire application
- Follow the existing style in `dashboard.py`
- Add a new function named `build_rep_leaderboard(df)`
- Add at least 3 pytest tests in `tests/test_dashboard.py`
- Make sure all existing tests still pass
- The dashboard must still generate `dashboard.html`

## Acceptance Criteria

The task is complete when:

- `dashboard.py` contains `build_rep_leaderboard(df)`
- The dashboard displays the new sales rep leaderboard section
- The leaderboard respects the quarter filter
- At least 3 tests verify the new function
- `pytest tests/ -v` passes
- `python dashboard.py` successfully generates `dashboard.html`