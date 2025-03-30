# Peer-Graded Assignment: Course Project 1

## Overview
Thank you for reviewing my submission. Please note that English is not my first language, so I appreciate your understanding.

## Repository Contents
This repository contains the following files:

1. **README.md** – Documentation and project details.
2. **R script** – The script used to generate the assignment plots.
3. **PNG image files** – The resulting plots from the analysis.

## Dataset
The dataset used for this project is **Electric Power Consumption** from the UCI Machine Learning Repository (approximately 20MB in size). You can download it from the official source.

### Description of Variables
The dataset contains 9 variables:

- **Date**: Date in the format `dd/mm/yyyy`.
- **Time**: Time in the format `hh:mm:ss`.
- **Global_active_power**: Household global minute-averaged active power (in kilowatts).
- **Global_reactive_power**: Household global minute-averaged reactive power (in kilowatts).
- **Voltage**: Minute-averaged voltage (in volts).
- **Global_intensity**: Household global minute-averaged current intensity (in amperes).
- **Sub_metering_1**: Energy sub-metering No. 1 (in watt-hours). Represents energy consumption in the kitchen (dishwasher, oven, microwave). Gas-powered hot plates are not included.
- **Sub_metering_2**: Energy sub-metering No. 2 (in watt-hours). Represents energy consumption in the laundry room (washing machine, tumble dryer, refrigerator, light).
- **Sub_metering_3**: Energy sub-metering No. 3 (in watt-hours). Represents energy consumption for an electric water heater and an air conditioner.

## Summary of Analysis
1. **Download Dataset**
2. **Load Data** – Extract data for the period from **February 1, 2007, to February 2, 2007**.
3. **Preprocess Data** – Convert variables into appropriate data types for visualization.
4. **Generate and Save Plots** – Create visualizations and save them as PNG files.

## Issue with Plots
There is an issue with **Plot 3 and Plot 4** where the legend is getting cut off in the saved PNG files. This problem does not occur when viewing the plots in an interactive window but appears when setting a specific image size while saving.

### Possible Causes & Solutions:
- The issue might be related to **plot margins or aspect ratio** settings.
- Adjusting **`mar` (margins) in `par()`** or using **`legend(x = "topright", inset = c(-0.1, 0))`** might resolve it.
- Saving with a higher resolution (`res=150` or more) in `png()` can help.
- Specifying a larger width and height when using `png()` could prevent truncation.

I appreciate any feedback or suggestions to improve this submission!

