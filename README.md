# Regional Sales MIS Tracker & Automated Reporting Dashboard

## 📊 Project Overview

The Regional Sales MIS Tracker is an Excel-based operational reporting tool designed to monitor regional sales performance against assigned targets.

The project uses Excel, Power Query, Pivot Tables, XLOOKUP, Conditional Formatting, Pivot Charts, and VBA automation to create a refreshable MIS reporting workflow.

The objective was to build a reporting tool that behaves like an operational MIS system rather than a one-time analysis.

---

## 🎯 Business Problem

Sales management needs regular visibility into:

- Regional sales performance
- Sales target vs actual achievement
- Monthly sales trends
- Underperforming regions
- Top-performing regions
- Overall sales growth
- Weekly reporting status

Manual reporting can require repeated data preparation, calculations, and dashboard updates.

This project creates a repeatable and refreshable reporting process using Excel automation.

---

## 🎯 Business Objectives

The MIS tracker was designed to:

1. Consolidate regional sales data.
2. Compare actual sales against sales targets.
3. Calculate target achievement percentage.
4. Identify regions below target.
5. Monitor monthly sales trends.
6. Provide management-level KPI visibility.
7. Reduce repetitive manual reporting work.
8. Provide a one-click refresh mechanism.
9. Maintain weekly reporting history.

---

## 📁 Dataset

The project uses a realistic dummy sales dataset created for portfolio purposes.

### Main Fields

| Column | Description |
|---|---|
| Date | Sales transaction date |
| Region | Sales region |
| Product | Product sold |
| Sales Target | Target assigned |
| Actual Sales | Actual sales achieved |
| Salesperson | Sales representative |

The dataset contains transaction-level sales records across multiple regions, products, and salespeople.

---

## 🏗️ Workbook Structure

### 1. `tbl_Sales`

Contains the structured operational sales data and acts as the primary source for the reporting pipeline.

### 2. `Pivot_Summary`

Contains:

- Region-wise Sales Target
- Region-wise Actual Sales
- Monthly Sales Target
- Monthly Actual Sales
- Target vs Achieved %
- Regional performance calculations

### 3. `Dashboard`

Management-facing dashboard containing:

- Total Sales
- Growth %
- Top Region
- Regional Sales vs Target chart
- Monthly Sales Trend chart
- Last Refreshed timestamp
- Refresh Data button

### 4. `Weekly_Status_Report`

Maintains manual historical snapshots of weekly MIS performance.

It records:

- Week Ending
- Total Sales
- Sales Target
- Achievement %
- Growth %
- Top Region
- Regions Below Target
- Key Observation
- Action Required
- MIS Prepared By

---

## 🔄 Reporting Workflow

```text
Operational Sales Data
          ↓
      Excel Table
          ↓
      Power Query
          ↓
    Refresh Data Button
          ↓
      Pivot Tables
          ↓
    KPI Calculations
          ↓
       Dashboard
          ↓
 Weekly Status Snapshot
