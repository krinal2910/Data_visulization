# Data_visulization
# Pymaceuticals Inc. Analysis

This project performs an in-depth analysis of drug efficacy in reducing tumor size in mice subjected to various treatment regimens. The data used in this analysis includes tumor volumes, metastatic sites, and mouse metadata. The goal is to identify potential drug treatments that show promise in controlling tumor growth.

## Table of Contents
- [Dependencies and Setup](#dependencies-and-setup)
- [Project Overview](#project-overview)
- [Data Files](#data-files)
- [Key Findings](#key-findings)
- [Summary Statistics](#summary-statistics)
- [Visualizations](#visualizations)
  - [Bar and Pie Charts](#bar-and-pie-charts)
  - [Quartiles, Outliers, and Boxplots](#quartiles-outliers-and-boxplots)
  - [Line and Scatter Plots](#line-and-scatter-plots)
- [Correlation and Regression](#correlation-and-regression)
- [Conclusion](#conclusion)

## Dependencies and Setup
The following libraries are required for running the analysis:
pip3 install matplotlib pandas scipy


# Project Overview
In this analysis, we assess tumor volumes for different drug regimens administered to mice. The data includes information such as mouse IDs, tumor volume, drug regimens, sex, and mouse age. This analysis includes statistical summaries, visualizations of key variables, and correlations between various factors like weight and tumor volume.

## Data Files
- **Mouse_metadata.csv**: Contains metadata for the mice in the study.
- **Study_results.csv**: Includes the tumor volume, metastatic sites, and other results related to the study. These files are combined to generate a single dataset for analysis.

## Key Findings
- A total of **248 unique mice** were used after removing duplicate entries.
- The study reveals potential outliers in the treatment regimens, with the **Infubinol** regimen showing one potential outlier.
- **Capomulin** and **Ramicane** show promising results with lower tumor volumes and no potential outliers.

## Summary Statistics
For each drug regimen, summary statistics are generated including:
- **Mean Tumor Volume**
- **Median Tumor Volume**
- **Tumor Volume Variance**
- **Tumor Volume Standard Deviation**
- **Tumor Volume Standard Error of Mean (SEM)**

##The statistics provide insights into how each drug regimen affects tumor growth.

## Visualizations
### Bar and Pie Charts
- **Bar Plot**: Shows the total number of timepoints for each drug regimen.
- **Pie Chart**: Visualizes the distribution of female and male mice in the study.

### Quartiles, Outliers, and Boxplots
The final tumor volume for each mouse across four treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin) is calculated.
- **Boxplots**: Display the tumor volume distribution for each drug regimen, highlighting potential outliers.

### Line and Scatter Plots
- **Line Plot**: Tumor volume over time for a single mouse treated with Capomulin is displayed.
- **Scatter Plot**: Shows the relationship between mouse weight and average tumor volume for the Capomulin regimen.

## Correlation and Regression
The correlation between mouse weight and tumor volume is calculated, showing a strong positive correlation (**0.84**). A linear regression model is fitted to describe this relationship.

## Conclusion
The analysis identifies key findings about the effectiveness of different drug regimens in controlling tumor growth. **Capomulin** and **Ramicane** regimens stand out as the most promising based on the summary statistics and visualizations.
