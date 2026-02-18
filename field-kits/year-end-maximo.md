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
