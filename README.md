# agentic-data-viz

⚡️ Drop your data. Let GitHub Copilot Agents handle the rest.

This repo showcases a zero-touch pipeline where CSV/JSON/XLSX files are checked in, GitHub Actions trigger issue creation, and Copilot Coding Agents automatically generate interactive HTML dashboards with insights.

---

## 🚀 What It Does

1. **Detects** data files (`.csv`, `.json`, `.xlsx`) on push to `main`
2. **Creates** an issue with a templated prompt for the Copilot Agent
3. **Assigns** the issue to GitHub Copilot (manually or in bulk)
4. **Copilot forks, builds, and submits a PR** with a full HTML report
---

## 🛠️ Setup

### 1. Fork or Clone This Repo

```bash
git clone https://github.com/YOUR-USER/agentic-data-viz.git
````

### 2. Add Your Data

Drop any of the following into the repo:

* `sales.csv`
* `data/sales.json`
* `hr/employees.xlsx`

### 3. GitHub Action

This repo includes a workflow:  
[`.github/workflows/data-file-issue.yml`](.github/workflows/data-file-issue.yml)
It triggers on data file check-in and creates an issue per file.

### 4. Assign Copilot

Once issues are created, go to the GitHub Issues tab.
Bulk-select → Assign to `copilot`.

Copilot will:

* Create branches
* Analyze data
* Generate HTML dashboards
* Submit pull requests for review

---

## 📊 Output Example

Each PR/brnach includes a file like:

```bash
employee-analysis.html
```

With:

* Summary insights
* Formatted data tables
* Charts (bar, pie, etc.)
* Visualized key metrics

---

## 🧠 Issue Prompt Template

The issue instructs Copilot to:

* Summarize the dataset
* Display a table of the data
* Create appropriate charts
* Output an interactive, standalone HTML page

You can customize this in [`.github/issue-template.md`](.github/issue-template.md).

---

## 📺 Demo Video

▶️ [Watch the walkthrough (8 min)](https://youtu.be/GKRG75JRZIE)

---

## 🧪 Sample Data

Included:

* `sales.csv`, `sales.json`, `sales.xlsx`
* `sales-dupes.csv` 
* `hr/employees.json`

---

## 🙌 Credits

Built by [Doug Finke](https://github.com/dfinke) using GitHub Copilot Coding Agents and GitHub Actions.

Stay curious.