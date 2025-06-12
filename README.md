# Client_Analysis_and_Gift_Cart_Allocation_With_Power_BI

Client Analysis and Gift Card Allocation – Power BI Dashboard

This Power BI project provides a detailed customer analysis based on demographic data, purchase behavior, and feedback. It also demonstrates advanced DAX usage by creating a custom *gift card* measure calculated from annual income and the number of children per household.

## 🎯 Project Objectives

- Analyze customer data: age, education level, income, marital status, and complaints.
- Understand purchasing behavior by channel (catalog, web, in-store).
- Create a dynamic KPI (gift card allocation) using DAX.
- Clean, transform, and visualize data effectively.

## 🧹 Data Preparation

- Removed unnecessary columns (reduced from 29 to 18).
- Converted ID from integer to text for privacy and clarity.
- Replaced 0/1 in Complaint column with No/Yes.
- Deleted empty rows and cells.
- Previewed and cleaned data in Excel before importing into Power BI.

## 🧮 DAX Measure Used

```dax
Gift Carts = SUM([Income]) * 0.002 * SUM([kidhome])
