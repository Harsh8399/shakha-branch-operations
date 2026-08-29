# Shakha — Branch Operations & Daily Reporting Dashboard

*"Shakha" (शाखा) is the Marathi/Hindi word for "branch" — this project simulates the daily coordination work of a branch back office.*

A browser-based dashboard that simulates how a back-office employee coordinates daily branch work: assigning and tracking tasks, monitoring team workload, and rolling up daily activity into reports.

**⚠️ All data in this project is sample/demo data** (fictional team members, tasks and figures) created for demonstration purposes only. No real branch, company or individual is represented.

---

## Problem

Day-to-day branch work — task assignment, deadlines, daily throughput — is often tracked informally, which makes it hard to see who's overloaded, what's overdue, or how a week of work actually adds up.

## Solution

Shakha gives a branch back office one place to manage tasks, see team workload at a glance, log a daily work report, and pull that data into daily/weekly/team-wise/status-wise reports — with CSV, print and PDF export.

## Key features

- **Dashboard** — a ledger-style tally strip (today's tasks, completed, pending, overdue, records processed today), a team workload chart and a task-status chart
- **Task & operation management** — Task ID, description, assigned person, priority, date, deadline, status and remarks, with full add/edit/delete; overdue tasks are detected automatically from the deadline
- **Team coordination** — every team member's assigned/completed/pending task counts with a workload gauge
- **Daily work report** — log records processed, documents verified, calls/emails handled, tasks completed and pending work for the day
- **Automatic summary** — total completed, total pending, completion rate and a productivity trend line chart, calculated live from the report history
- **Reports** — Daily, Weekly, Team-wise and Status-wise views, each exportable to CSV, printable, or downloadable as a one-page PDF summary
- **Search, filter & sort** on the task register; validation and error handling throughout

## Technology stack

- HTML5 + hand-written CSS (CSS custom properties for theming — no UI framework)
- Vanilla JavaScript (ES6+), no build step
- [Chart.js](https://www.chartjs.org/) via CDN for charts
- [jsPDF](https://github.com/parallax/jsPDF) via CDN for the one-click PDF summary
- Browser `localStorage` for persistence — no backend or database required

## Skills this demonstrates for a Back Office Executive role

| JD requirement | Where it shows up |
|---|---|
| Supporting day-to-day branch operations | The entire task/operations dashboard |
| Coordinating with team members | Team Coordination module with workload tracking |
| Managing office files, documents & reports | Daily/weekly/team/status reports with CSV, print & PDF export |
| Data entry & maintaining accurate records | Daily work-report form with numeric validation |
| Attention to detail | Deadline validation, automatic overdue detection, confirmation dialogs |

## Installation & running it

No build tools or server required.

1. Download or clone this folder.
2. Open `index.html` directly in any modern browser.
3. **Recommended:** deploy to **GitHub Pages**, or open via VS Code's "Live Server" extension for the smoothest `localStorage` behaviour.

On first load the app seeds itself with sample tasks and four days of sample daily reports. Use **"Reset sample data"** in the top bar to restore the originals at any time.

## Usage

1. **Dashboard** — check today's tally strip and charts.
2. **Tasks & Operations** — add, edit, filter, or sort tasks; overdue ones are flagged automatically.
3. **Team Coordination** — see each member's active workload.
4. **Daily Work Report** — log today's numbers; the summary and trend chart update immediately. Click **Edit** on any past entry to update it.
5. **Reports** — switch between Daily / Weekly / Team-wise / Status-wise, then export CSV, print, or download a PDF summary.

## Project structure

```
shakha-branch-operations-dashboard/
├── index.html   # all markup, styling and app logic in one file (portable, zero-build)
└── README.md
```

## Future improvements

- Replace `localStorage` with a shared backend so the whole branch team sees the same live data
- Add authentication so each team member only edits their own tasks
- Push overdue-task alerts (email/SMS) instead of relying on the dashboard being open
- Multi-branch roll-up reporting for a regional back-office view

## Screenshots

*(Add screenshots here after running the app — see the portfolio guide for a recommended shot list.)*
