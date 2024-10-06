# Matplotlib
Project Overview

This project analyzes data from 249 mice that were identified with SCC tumors and received treatment with various drug regimens. Over a period of 45 days, tumor growth and development were measured to assess the effectiveness of different treatments. The primary focus of the study was to evaluate Pymaceuticals' drug of interest, Capomulin, in comparison to other available treatment regimens.

Files in the Repository
This repository contains the following key files:

Mouse_metadata.csv - Contains information about each mouse, including Mouse ID, Drug Regimen, Sex, Age, and Weight.

Study_results.csv - Records the Timepoint, Tumor Volume, and Metastatic Sites for each Mouse ID.

These two files are located in the Data directory.

pymaceuticals_starter.ipynb - The main script that processes the data and generates visualizations.

How the Script Works
The script reads data from the Mouse_metadata.csv and Study_results.csv files in the Data directory. It performs the following steps:

1. Data Processing and Calculations: Merges the datafiles and study results into a single DataFrame. Generates summary statistics for each drug regimen, including:
Mean, median, variance, standard deviation, and standard error of the mean (SEM) for tumor volumes.
Analyzes the interquartile range (IQR) of tumor volumes for the most promising treatments: Capomulin, Ramicane, Infubinol, and Ceftamin, to detect any potential outliers.
Calculates the correlation coefficient between mouse weight and the average tumor volume specifically for the Capomulin regimen.

3. Data Visualization:
The script generates the following visualizations using Matplotlib and Pandas:

Bar Chart:Displays the total number of timepoints (Mouse ID/Timepoint pairs) for each drug regimen throughout the study.

Pie Chart:Shows the distribution of male versus female mice involved in the study.

Box Plot:Illustrates the distribution of final tumor volumes for all mice across different treatment groups, with potential outliers.

Line Plot:Tracks the tumor volume over time for a specific mouse treated with Capomulin, showing how the tumor responded to the drug.

Linear Regression Model:A scatter plot with a linear regression line that demonstrates the relationship between mouse weight and average tumor volume for the Capomulin regimen.

How to Run the Script
Prerequisites:
Ensure that you have Pandas and Matplotlib installed in your Python environment.

Steps to Run:

Place the Mouse_metadata.csv and Study_results.csv files in a folder named Data located in the same directory as the pymaceuticals_starter.ipynb script.
Open the Jupyter Notebook and execute the cells in order to generate the required DataFrames, perform statistical analyses, and produce visualizations.

Drug Testing Analysis:
Capomulin was the most frequently tested drug, followed by Ramicane, while Propriva was the least observed in the study.
The number of male and female mice used in the testing was nearly equal.
A positive correlation was observed between the average tumor volume and the weight of the mice. As the mice's weight increased, the tumor volume also increased.
