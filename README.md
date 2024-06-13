# Analysis-of-Parking-Contraventions-Dataset

## Project Context

The Winnipeg Parking Authority provides a comprehensive dataset of parking contraventions issued from 2010 to the present. This dataset includes detailed information about each citation, including geolocation data, the specific bylaw violated, and the corresponding fines. The primary goal of this project is to analyze this dataset to identify patterns, trends, and insights that can help improve parking policies, enforcement strategies, and public awareness.

## Project Objectives

1. **Identify Temporal Trends**: Analyze the distribution of parking violations over time to identify peak periods for violations.
2. **Geospatial Analysis**: Determine hotspots for parking violations across Winnipeg using geolocation data.
3. **Fine Analysis**: Evaluate the financial impact of parking violations by examining the distribution and trends of fines issued.
4. **Bylaw Violation Analysis**: Investigate which bylaws are most frequently violated to provide insights into potential areas for policy improvement.
5. **Payment Behavior Analysis**: Assess the effectiveness of the early payment discount in encouraging timely fine payments.

## Dataset Overview

- **Dataset Name**: Parking Contravention (Citations)
- **Data Source**: Open Data Services, Winnipeg Parking Authority
- **Date Range**: Starting from 2010
- **Last Updated**: June 10, 2024
- **Rows**: 1.9 million
- **Columns**: 7

### Dataset Columns

1. **Issue Date (issue_date)**: Date and time when the violation was issued.
2. **Violation (violation)**: Description of the bylaw that was violated.
3. **Street (street)**: The street where the violation occurred.
4. **Location (location)**: General area where the violation occurred.
5. **Discounted Fine (discounted_fine)**: The fine amount if paid early.
6. **Full Fine (full_fine)**: The full fine amount if not paid early.
7. **Point (point)**: Geolocation data (latitude and longitude) of the violation.

## Problem Statement

The City of Winnipeg seeks to optimize parking management and enforcement to reduce the number of parking violations and improve compliance with parking regulations. However, the current data is underutilized in forming effective policies and strategies.

## Proposed Solution

Conduct a detailed analysis of the Parking Contraventions dataset to uncover actionable insights that can guide policy improvements and enforcement strategies.

## Analysis Plan

### Data Preparation

1. Import the dataset into a SQL database.
2. Clean the data by handling missing values and standardizing formats.
3. Create indexes on frequently queried fields (e.g., `issue_date`, `violation`, `point`) to improve query performance.

### Temporal Analysis

1. Use SQL queries to aggregate violation counts by year, month, and day of the week.
2. Identify trends and seasonal patterns in parking violations.

### Geospatial Analysis

1. Utilize SQL's spatial functions to map the distribution of violations.
2. Identify hotspots using clustering algorithms like K-means or DBSCAN.

### Fine Analysis

1. Calculate the total revenue from fines per year.
2. Compare the distribution of full fines vs. discounted fines to assess payment behavior.

### Bylaw Violation Analysis

1. Rank violations by frequency to identify the most common infractions.
2. Analyze the relationship between specific violations and their locations.

### Payment Behavior Analysis

1. Evaluate the proportion of fines paid early versus late.
2. Determine if certain violations are more likely to be paid early.

---

