---
layout: page
title: "Maximo Year-End Processing Checklist"
permalink: /field-kits/year-end-maximo/
description: "Step-by-step Maximo year-end processing guide to ensure system readiness for the new year."
---

Year-end is one of the busiest times of the year. Many activities need to be completed and closed out quickly. Maximo is just one of them, but it can easily be forgotten in the end-of-year shuffle.

A few simple preparation tasks will ensure that Maximo is ready for the new year — and that you won’t be fielding emergency calls on New Years’ Day.

---

## Key Activities

- Reset and roll over inventory issue history  
- Reset and roll up asset costs  
- Reset labor hours  
- Update financial periods  
- Update calendars  
- Update auto-number sequences  

> **Note:** Depending on your configuration, you may have additional year-end processing to support system interfaces, particularly financial system integrations.

We’ve demonstrated several of the most common year-end tasks below. To simplify the process even further, automating year-end processing is strongly recommended.

---

## Inventory Issue History

Use the **Zero Year to Date Quantities** action to set Year-to-Date inventory issues to zero and roll each year’s totals to the previous year.

### Steps

1. Navigate to the **Inventory Application**
2. Hit **Enter** to bring up all records

> **Best Practice:** Review Issue History of one record to validate results before proceeding.

3. Return to List View when finished
4. From the Actions menu select:  
   `More Actions > Inventory Adjustments > Zero Year to Date Quantities`
5. Confirm the action by clicking **OK**

> **Best Practice:** Review Inventory Issue History and verify Year-to-Date totals have been set to zero and prior year totals have been advanced.

---

## Reset Asset Year-to-Date Costs

### Steps

1. Navigate to the **Asset Application**
2. In the Advanced Search dropdown, open the **Where Clause**
3. Enter the following query to bring up only assets with YTD costs:

(ytdcost != '0')


> **Best Practice:** Review YTD Costs of one record to validate results before applying changes system-wide.

4. Return to List View when finished
5. From the Actions menu select:  
`More Actions > Zero Asset Costs`
6. Confirm the update to all listed records by clicking **OK**
7. When prompted:
- Select **Zero Year to Date Costs?**
- Click **OK**

> **Note:** The system may take time to complete the process depending on record volume.

> **Best Practice:** Review Asset Costs afterward to verify YTD Cost has been set to zero.

---

## Labor Hours

Navigate to:

**Administration > Resources > Labor**

### Steps

1. Open the **Labor Application**
2. Under **More Actions**, select **Zero Year to Date Hours**

---

## Financial Periods

If your financial periods are defined by calendar year, you must add a new period for the upcoming year.

If a valid financial period is not defined, users will be unable to:

- Record labor  
- Issue inventory  
- Receive inventory  
- Adjust inventory  

They will receive the following error:

> **Warning:** `BMXAA1198E – The date is not within a valid financial period.`

### To Update Financial Periods

1. Navigate to:  
**Financial > Chart of Accounts**
2. From the **More Actions** menu, select **Financial Periods**
3. Add a new row for the next financial period

### Example Entry

| Field  | Value           |
|--------|-----------------|
| Period | 2022            |
| From   | 1/1/22 12:00 AM |
| To     | 1/1/23 12:00 AM |

> **Important:** Do not enter Accounting Close Date or Actual Close Date until you plan to close the period.

---

## Other Tasks

In addition to the tasks outlined above:

- Review all year-end activities listed in the introduction  
- Check with your team to determine whether additional processing is required  
- Pay special attention to ERP integrations  

> **Recommendation:** If you haven’t already, consider using **Maximo Escalations** to automate year-end processing in the future.

---

Proactive preparation ensures a smooth transition into the new year and prevents avoidable system disruptions.
