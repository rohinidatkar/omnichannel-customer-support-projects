# Omnichannel Customer Support Projects

Three self-built projects aligned with omnichannel customer service roles: SLA tracking, written communication, and complaint analysis.

| # | Project | Tools | Notebook |
|---|---------|-------|----------|
| 1 | Omnichannel Support Ticket Tracker | Python, SQL (SQLite), Excel, Power BI | `01_omnichannel_ticket_tracker/omnichannel_ticket_tracker.ipynb` |
| 2 | Customer Email and Chat Response Playbook | Python, written communication | `02_email_chat_response_playbook/email_chat_response_playbook.ipynb` |
| 3 | Customer Satisfaction and Complaint Analysis | Python, Excel, Power BI / Tableau | `03_customer_satisfaction_complaint_analysis/customer_satisfaction_complaint_analysis.ipynb` |

## 1. Omnichannel Support Ticket Tracker
- Builds a 600-ticket log across **email, chat and phone** with priority, status, resolution time and SLA due date.
- Flags **SLA breaches** and **overdue pending tickets** (the "chase list").
- SQL queries for SLA adherence by channel, breaches by priority and overdue tickets.
- Weekly summary of **volume, resolution time and SLA adherence** against a 90% target.
- Exports `ticket_log.csv`, `weekly_summary.csv` and `ticket_tracker.xlsx` for Power BI (DAX measures included in the notebook).

## 2. Customer Email and Chat Response Playbook
- Email and chat replies for **delayed delivery, refund requests, billing errors, angry customers** and wrong/damaged items.
- **Escalation matrix**: when to escalate, to whom and the expected response time.
- Standard **resolution approach** for each scenario.
- Rule-based **reply-quality checker** (greeting, empathy, ownership, next step with timeline, closing).
- Exports `playbook.md` and CSVs.

## 3. Customer Satisfaction and Complaint Analysis
- Categorises complaints and tracks **resolution rate, timely response, recurring issues** and month-by-month trends.
- Pareto of top issues and a growth check (last 3 months vs prior 3).
- Short, issue-specific **recommendations** to reduce repeat complaints.
- Exports clean CSVs and an Excel workbook for a Power BI / Tableau dashboard.

## How to run
```bash
pip install -r requirements.txt
jupyter notebook
```
Open each notebook and choose **Kernel -> Restart & Run All**. Each notebook writes its outputs to a `data/` or `output/` folder next to it. Sample outputs from one run are already included.

## Data (please read)
- Projects 1 and 2 use **sample/synthetic data and sample scenarios** written for this portfolio. They contain no real customer data.
- Project 3 runs on a **synthetic sample** by default. To use real public data, download the CSV from the [CFPB Consumer Complaint Database](https://www.consumerfinance.gov/data-research/consumer-complaints/), save it as `03_customer_satisfaction_complaint_analysis/data/complaints_public.csv`, and re-run. Describe the project as built on public data only after doing this.
- Escalation thresholds (Rs amounts, hours) in Project 2 are sample values, not any company's real policy.

## Power BI / Tableau
The notebooks prepare the data and list the DAX measures and dashboard layout. The dashboard files (`.pbix` / Tableau workbook) need to be built in those tools from the exported CSVs; add screenshots to a `screenshots/` folder and link them here.

## Resume-to-project mapping
| Resume line | Where it is shown |
|---|---|
| Ticket log with priority, status, resolution time, SLA due date | Project 1, section 1 |
| Flagged SLA breaches and pending tickets | Project 1, sections 2-3 |
| Weekly summary dashboard | Project 1, section 4 |
| Professional email/chat replies for common scenarios | Project 2, section 1 |
| Escalation matrix and standard resolution approach | Project 2, sections 2-3 |
| Complaint categories, resolution rate, recurring issues | Project 3, sections 2-4 |
| Dashboard and recommendations for reducing repeat complaints | Project 3, sections 7-8 |
