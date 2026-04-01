# AI Agent Weekly Research Repo

This repository is set up to save a weekly AI agent research report into GitHub by date.

## What it does
- Runs once a week with GitHub Actions
- Uses the Codex GitHub Action to generate a report
- Saves the result into a date-based folder such as `reports/2026/2026-04-06/`
- Commits the generated files back to the repository automatically

## Files generated each run
- `reports/YYYY/YYYY-MM-DD/summary.md`
- `reports/YYYY/YYYY-MM-DD/signals.json`
- `reports/latest/summary.md`
- `reports/latest/signals.json`
- `reports/index.md`

## Setup
1. Create a GitHub repository and upload these files.
2. In the repository settings, add a secret named `OPENAI_API_KEY`.
3. Enable GitHub Actions for the repository.
4. Optionally adjust the cron schedule in `.github/workflows/weekly-agent-research.yml`.

## Schedule
The workflow is configured for every Monday at 00:10 UTC, which is Monday 09:10 in Japan Standard Time. GitHub schedules run in UTC and notes that scheduled workflows can be delayed during high-load periods, especially around the top of the hour, so the workflow uses 00:10 instead of exactly 00:00 UTC.

## Notes
- The current ChatGPT scheduled task cannot directly push files into your GitHub repository by itself. This repo-based workflow is the practical way to get dated deliverables committed automatically.
- The prompt tells Codex to research AI agents broadly, not just Codex.
