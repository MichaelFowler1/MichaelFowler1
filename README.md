# Hi, I'm Michael Fowler

I'm an operations research analyst in defense cost estimating. For the last three years I've built life-cycle cost estimates, tracked earned value and checked schedules for Navy aviation acquisition programs, and I write Python for the parts of that job that shouldn't be done by hand.

Most of my time on GitHub goes to two open-source tools. Both are built for the way cost work actually gets done: in Excel, by a team, with numbers someone will have to defend in a review.

## cost-core

**[cost-core](https://github.com/MichaelFowler1/cost-risk-toolkit)** does the analysis a cost shop runs every month, from one command, `ce-core`.

- **Cost risk.** Put an estimate in Excel with a low, most likely and high for each WBS element. You get the S-curve, the chance the estimate is exceeded, what it takes to be 80% sure, which elements drive the spread, and the P80 reserve shared out across the WBS.
- **Earned value.** Forecasts final cost and finish from a spreadsheet or an IPMDAR delivery, with earned schedule, independent EACs, variance thresholds and the monthly data checks.
- **Schedules.** The DCMA 14-point check on a Microsoft Project file, and joint cost and schedule confidence (JCL).
- **The rest of the toolbox.** Learning curve and rate fits for production lots, analysis of alternatives on life-cycle cost, choosing a portfolio within a budget, and base-year to then-year conversion with the index you supply.

Every run reads Excel and writes a `report.xlsx` and a `brief.pptx`, says what the result means in plain words and writes down every assumption it made. It runs on your own machine and sends nothing anywhere. As far as I can find, it's the first public Python package that does all of these together.

```bash
pip install cost-core
ce-core demo cost-risk
```

[cost-core-starter](https://github.com/MichaelFowler1/cost-core-starter) has example workbooks ready to run. It's free for noncommercial use and for U.S. government work, contractors included ([the licence](https://github.com/MichaelFowler1/cost-risk-toolkit#license) has the details).

If you'd rather click than type commands, [lot-cost-model](https://github.com/MichaelFowler1/lot-cost-model) puts the learning-curve side of cost-core in a desktop window: type in your production lots, click Run, and get back an Excel workbook with the fit, the lot-by-lot projections and the charts.

## xlgit

**[xlgit](https://github.com/MichaelFowler1/excel-git)** is git diff and merge for Excel. Two people edit the same workbook on their own branches, and git merges it cell by cell. Charts, tables, pivot tables and macros come through intact, and only a cell you both changed is a conflict.

`git diff` shows `Budget!B2 1000 -> 1100` instead of "Binary files differ", and the [GitHub Action](https://github.com/marketplace/actions/excel-diff-xlgit) comments every changed cell, chart and pivot on a pull request. As far as I know it's the only free, open-source tool that merges two versions of a workbook automatically and keeps everything in it working. It's still beta, fuzz-tested against about 3,000 real workbooks, and Apache-2.0.

```bash
pip install xlgit
xlgit demo
```

## Why these two

On most teams a cost model is a workbook that gets emailed around until someone's copy is called `estimate_v7_FINAL.xlsx`. xlgit puts that workbook under version control so two analysts can work on it at once and see exactly what the other changed. cost-core runs the risk, EVM and schedule analysis on it. Between them, an estimate gets the same history and review that code does.

## What I know

- **Cost estimating:** life-cycle cost estimates, CERs and regression, learning curves and rate effects, inflation and quantity normalization, CSDR and FlexFile data.
- **Earned value and schedule:** IPMDAR surveillance, independent EACs, DCMA 14-point assessments, schedule risk analysis, JCL.
- **Risk:** Monte Carlo cost and schedule risk, correlation across the WBS, S-curves and confidence-level funding.
- **Code:** Python (pandas, NumPy, SciPy), SQL, Power Query, Git and CI, and locally hosted LLMs for data that can't leave the building.

MS in Systems Analysis from the Naval Postgraduate School, with graduate certificates in cost estimating and analysis and in systems analysis. BS in Information Systems from UMBC.

Everything here is a personal project, built on my own time and equipment. None of it is endorsed by the Navy, the Department of Defense or any employer.

Find me on [LinkedIn](https://www.linkedin.com/in/michaelfowlerii), or open an issue on any repo.
