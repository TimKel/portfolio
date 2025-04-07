---
title: "Revenue Reporting in Tons: A Twist on Traditional Dashboards"
description: "Revenue Reporting in Tons: A Twist on Traditional Dashboards"
date: "2025-04-06"
banner:
  src: "../../images/salesDashboardWithToolTips.png"
  alt: "Sales Dashboard Photo"
  caption: 'Report developed by <u>Tim Kelley</u>'
categories:
  - "Power BI"
  - "Data-Warehouse"
  - "Revenue Reporting"
  - "SAP"
keywords:
  - "Azure Synapse"
  - "SAP"
  - "Data-Warehouse"
  - "SQL"
  - "Power BI"
  - "DAX"
  - "ALM Toolkit"
---

## Technologies Used:
Power BI - SQL - SSMS - ALM Toolkit - Azure Synapse

## The Client:
This client is a trusted supplier in the mining industry. Reports developed were largely Operations and Revenue. Tracking how a foundry conducts melts and building reporting around chemistry details was quite the learning experience.

## Overview:

This report was designed to provide revenue visibility, but with a twist. The client needed to track performance in both dollars, and tons as they're a mining and melting company. They also needed to split tonnage by Metric and US tons. Additionally, they required a separation of closed revenue vs open revenue. All of this in comparison to Revenue Plan, needing to be sliced by different categories like Product and Customer.  

## Process:

Data was extracted from SAP into a custom-built data warehouse, where it's transformed and loaded into Power BI. To keep report performance fast, I broke key metrics down into optimized DAX measures using variables, and utilized `SWITCH` statements to create the functionality requests mentioned above. I also used Calculation Groups to reduce redundancy for values like SPLY measures. Lastly, I implemented bookmarks to toggle between a monthly and quarterly view based on the selected date range. 

## Custom Tooltips:

To enhance insight and usability, I built a custom tooltip. When an employee hovers over the four category slices on the bottom left, they get additional detail on how that specific product, customer, etc is performing against their individual plans. 

![This is the alt tag.](../../images/CustomToolTip.png "Example of the custom tooltip I built.")

## Adoption:

After publishing, I built a custom Usage Metrics Report so the client could track adoption of all reporting. This report quickly became one of their most-used tools alongside a gross margin version I also created. In total, I developed 5-6 different report suites for this client, each containing 3-5 pages on average. 

