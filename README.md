# Daily Automated Naukri Job Applicator & Profile Booster

An automated tool configured for **Gnana Kumar S**, focused on **SAP ABAP Consultant**, **ABAP on HANA**, **RICEF**, **CDS Views**, **OData**, **SAP Workflow**, and **SAP S/4HANA** jobs in **Bengaluru** and **Remote** locations.

---

## Features

1. **Dry-run and live modes**: Test job matches without applying before enabling applications.
2. **Persistent login session**: Interactive one-time login saves the local browser session.
3. **SAP-focused search**: Searches the configured SAP ABAP keywords and locations.
4. **Application audit**: Tracks applications and external/company-site skips.
5. **Windows scheduling and GitHub Actions support**: Runs locally or in a cloud workflow.

---

## Setup

```powershell
Set-Location "C:\Users\Lumbini_User\Desktop\VS CODE\job"
& ".\.venv\Scripts\python.exe" -m pip install -r requirements.txt
& ".\.venv\Scripts\python.exe" -m playwright install chrome
& ".\.venv\Scripts\python.exe" login.py
```

After login, verify without submitting applications:

```powershell
& ".\.venv\Scripts\python.exe" bot.py --dry-run
```

Live mode is disabled while `dry_run` is `true` in `config.json`.
