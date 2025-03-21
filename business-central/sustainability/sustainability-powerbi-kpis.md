---
title: Sustainability KPIs and measures (Power BI)
description: Get an overview of all the KPIs and measures in the semantic model for the Sustainability Power BI app.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 10/26/2024
ms.service: dynamics-365-business-central
---

# Power BI Sustainability app KPIs and measures

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Sustainability report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

## Emission Fees Table

**Emissions Fees Measures**
- [Metric One](#metric-one)

### Metric One
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

## Employee Absences Table

**Employee Absences Measures**
- [Metric One](#metric-one)

### Metric One
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

## Employee Ledger Entries Table

**Employee Ledger Entries Measures**
- [Metric One](#metric-one)

### Metric One
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

## Employee Qualifications Table

**Employee Qualifications Measures**
- [Metric One](#metric-one)

### Metric One
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

## Employee Table

**Employee Measures**
- [Metric One](#metric-one)

### Metric One
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

## Responsibility Centre Table

**Responsibility Centre Measures**
- [Facility Capactity](#facility-capactity)

### Facility Capactity
**Formula**  
Measures the water capacity of the facility (Responsibilty Centre)

**Data Sources**
- Responsibility Centre

## Sustainability Goals Table

**Sustainability Goals Measures**
- [CH4 Target](#ch4-target)
- [CO2 Target](#co2-target)
- [N2O Target](#n2o-target)
- [Waste Target](#waste-target)
- [Water Target](#water-target)


### CH4 Target
**Formula**  
Sum of Target Value for CH4 from the Sustainabilty Goals.

**Data Sources**
- Sustainability Goals

### CO2 Target
**Formula**  
Sum of Target Value for CH4 from the Sustainabilty Goals.

**Data Sources**
- Sustainability Goals

### N2O Target
**Formula**  
Sum of Target Value for N2O from the Sustainabilty Goals.

**Data Sources**
- Sustainability Goals

### Waste Target
**Formula**  
Sum of Target Value for Waste from the Sustainabilty Goals.

**Data Sources**
- Sustainability Goals

### Water Target
**Formula**  
Sum of Target Value for Water from the Sustainabilty Goals.

**Data Sources**
- Sustainability Goals

### Realized (%) for CH4
**Formula**  
Realized (%) for CH4 = [Net Change CH4](#net-change-ch4) / [CH4 Target](#ch4-target)

**Data Sources**
- Sustainability Goals
- Sustainability Ledger Entry


### Realized (%) for CO2
**Formula**  
Realized (%) for CO2 = [Net Change CO2](#net-change-co2) / [CO2 Target](#co2-target)

**Data Sources**
- Sustainability Goals
- Sustainability Ledger Entry


### Realized (%) for N2O
**Formula**  
Realized (%) for N2O = [Net Change N2O](#net-change-n20) / [N2O Target](#n2o-target)

**Data Sources**
- Sustainability Goals
- Sustainability Ledger Entry


### Realized (%) for Waste
**Formula**  
Realized (%) for Waste = [Net Change Waste](#net-change-waste-intensity) / [Waste Target](#waste-target)

**Data Sources**
- Sustainability Goals
- Sustainability Ledger Entry

### Realized (%) for Water
**Formula**  
Realized (%) for Water = [Net Change Water](#net-change-water-intensity) / [Water Target](#water-target)

**Data Sources**
- Sustainability Goals
- Sustainability Ledger Entry

## Sustainability Ledger Entries Table

**Sustainability Ledger Entries Measures**
- [Net Change CH4](#net-change-ch4)
- [Balance at Date CH4 Emissions](#balance-at-date-ch4-emissions)
- [Balance CH4 Emissions](#balance-ch4-emissions)
- [Net Change CO2](#net-change-co2)
- [Balance at Date CO2 Emissions](#balance-at-date-co2-emissions)
- [Balance CO2 Emissions](#balance-co2-emissions)
- [Net Change N2O](#net-change-n2o)
- [Net Change CO2e](#net-change-co2e)
- [Net Change Discharged Into Water](#net-change-discharged-into-water)
- [Net Change Water Intensity](#net-change-water-intensity)
- [Net Change Waste Intensity](#net-change-waste-intensity)


### Net Change CH4
**Formula**  
Sum of CH4 from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date CH4 Emissions
**Formula**  
The Balance at Date CH4 Emissions measure calculates the cumulative [Net Change CH4](#net-change-ch4) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance CH4 Emissions
**Formula**  
The Balance measure calculates the total [Net Change CH4](#net-change-ch4) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change CO2
**Formula**  
Sum of CO2 from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date CO2 Emissions
**Formula**  
The Balance at Date CO2 Emissions measure calculates the cumulative [Net Change CO2](#net-change-co2) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance CO2 Emissions
**Formula**  
The Balance measure calculates the total [Net Change CO2](#net-change-co2) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change N2O
**Formula**  
Sum of N2O from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date N2O Emissions
**Formula**  
The Balance at Date N2O Emissions measure calculates the cumulative [Net Change N2O](#net-change-n20) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance N2O Emissions
**Formula**  
The Balance measure calculates the total [Net Change N2O](#net-change-n20) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change CO2e
**Formula**  
Sum of CO2e from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry


### Balance at Date CO2e Emissions
**Formula**  
The Balance at Date CO2e Emissions measure calculates the cumulative [Net Change CO2e](#net-change-co2e) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance CO2e Emissions
**Formula**  
The Balance measure calculates the total [Net Change CO2e](#net-change-co2e) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change Discharged Into Water
**Formula**  
Sum of Discharged into Water from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date Discharged Into Water
**Formula**  
The Balance at Date Discharged Into Water measure calculates the cumulative [Net Change Discharged Into Water](#net-change-discharged-into-water) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance Discharged Into Water
**Formula**  
The Balance measure calculates the total [Net Change Discharged Into Water](#net-change-discharged-into-water) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change Water Intensity
**Formula**  
Sum of Water Intensity from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date Water Intensity
**Formula**  
The Balance at Date Water Intensity measure calculates the cumulative [Net Change Water Intensity](#net-change-water-intensity) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance Water Intensity
**Formula**  
The Balance Water Intensity measure calculates the total [Net Change Water Intensity](#net-change-water-intensity) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

### Net Change Waste Intensity
**Formula**  
Sum of Waste Intensity from the Sustainability Ledger Entry.

**Data Sources**
- Sustainability Ledger Entry

### Balance at Date Waste Intensity
**Formula**  
The Balance at Date Discharged Into Water measure calculates the cumulative [Net Change Water Intensity](#net-change-waste-intensity) up to the latest date in the current filter context. It removes all date filters, then re-applies a filter to include only dates up to and including the maximum date within the selection. This provides a running balance up to the specified date.

**Data Sources**
- Sustainability Ledger Entry

### Balance Waste Intensity
**Formula**  
The Balance measure calculates the total [Net Change Waste Intensity](#net-change-waste-intensity) across all dates, ignoring any filters on the Date table. By removing date-based filtering, this measure provides the full net change value from the start to the end of the dataset, regardless of any date selections applied in the report.

**Data Sources**
- Sustainability Ledger Entry

**Baseline Calculation Measures**

