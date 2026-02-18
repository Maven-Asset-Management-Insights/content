---
layout: default
title: Year-End Maximo Preparation Checklist
permalink: /field-kits/year-end-maximo/
---

# Year-End Maximo Preparation Checklist

Year-end is one of the busiest times of the year. Between financial closeout, reporting, audits, and operational demands, Maximo maintenance tasks can easily be forgotten in the shuffle.

A few simple preparation activities will ensure Maximo is ready for the new year — and help prevent emergency support calls on New Year’s Day.

---

## Key Activities Include

- Reset and roll over inventory issue history
- Reset and roll up asset costs
- Reset labor hours
- Update financial periods
- Update calendars
- Update auto-number sequences

> Depending on your configuration, additional year-end processing may be needed for system interfaces (especially financial/ERP integrations).

Maven strongly recommends automating year-end processing whenever possible.

---

## Inventory Issue History

Use the **Zero Year to Date Quantities** action to set Year-to-Date inventory issues to zero and roll each year’s totals forward.

### Steps

1. Navigate to the **Inventory** application
2. Hit **Enter** to bring up all records
3. *(Optional Best Practice)* Review Issue History of one record to validate results
4. Select: **More Actions → Inventory Adjustments → Zero Year to Date Quantities**
5. Confirm the action by clicking **OK**
6. *(Optional Best Practice)* Review Inventory Issue History to verify YTD totals have been set to zero and prior year totals have advanced

---

## Reset Asset Year-to-Date Costs

### Steps

1. Navigate to the **Asset** application
2. In the Advanced Search dropdown, open the **Where Clause**
3. Enter this query to bring up only assets with YTD costs:

```sql
(ytdcost != '0')
(Optional Best Practice) Review YTD Costs of one record to validate results

Select: More Actions → Zero Asset Costs

Confirm the update to all listed records by clicking OK

Select: Zero Year to Date Costs? → Click OK

The system may take time to complete depending on record volume

(Optional Best Practice) Review Asset Costs to confirm YTD Cost has been set to zero

Labor Hours

Navigate to the Labor application: Administration → Resources → Labor

Under More Actions, select: Zero Year to Date Hours

Financial Periods

If your financial periods are defined by calendar year, be sure to add a new period for the upcoming year.

If a new financial period is not defined, users may be unable to record labor, issue inventory, receive inventory, or adjust inventory — and may receive:

BMXAA1198E – The date is not within a valid financial period.

Steps

Navigate to: Financial → Chart of Accounts

From the More Actions menu, select: Financial Periods

Enter a new row for the next period (example values):

Period: 2022

From: 1/1/22 12:00 AM

To: 1/1/23 12:00 AM

Do not enter Accounting Close Date or Actual Close Date until you plan to close the period.

Other Recommended Tasks

In addition to the tasks above, consider reviewing:

calendars

auto-number sequences

integration processes (especially ERP/financial integrations)

If you haven’t already, consider using Maximo Escalations to automate year-end processing going forward.
