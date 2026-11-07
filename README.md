# 200-Day AI Engineering Challenge

## About This Project
This repository documents my 200-day journey toward becoming an AI Engineer. I am developing practical skills in Python, data analysis, machine learning, deep learning, and AI agents through hands-on projects.

## Project 1: Python Automation & Data Analysis Toolkit

### Day 1 — Distance Converter
Built a Python function to convert distances from miles to kilometers.

### Day 2 — Python Testing
Practiced automated testing, debugging, and protecting original input lists from unintended changes.

### Day 3 — Distance Summary Analyzer
Created a Python notebook to analyze distances using functions, loops, accumulators, and dictionaries.

Features:
- Convert miles into kilometers
- Calculate total distance
- Calculate average distance
- Identify the longest distance
- Handle empty input lists

## My Goal
Build four significant AI engineering portfolio projects and develop the skills needed for an entry-level technology career.

## Day 4 — Data Cleaning

Built a Python function called clean_distances() to remove negative distance values while preserving the original dataset.

Features:
- Remove negative distances.
- Keep zero and positive numbers.
- Use for loops and conditional statements.
- Use .append() to build a new list.
- Preserve the original list.
- Verify functionality using automated tests.

What I learned:

I practiced Python functions, loops, list accumulation, and automated testing. I also learned why keeping original data unchanged is important in data preprocessing and machine learning.

## Day 5 - export clean distances
I created a python fuction that clean a list of distances, create a csv file and return a clean list of distances.
I tested if it works with a list of values without changing the original list, and that work with and empty list.
### Day 6 — CSV Statistics

The function `summarize_distances_csv(filename)`:

- Reads distance measurements from a CSV file.
- Skips the header and converts distance strings into numbers.
- Counts the number of distances.
- Calculates the total distance in miles.
- Calculates the average distance in miles.
- Handles empty datasets without division-by-zero errors.
- Returns the statistics in a dictionary.
- Preserves the original CSV file.

**What I learned:** I practiced reading CSV files, using Python functions, converting data types, calculating summary statistics, and testing my code.
## Day 7: Add CSV data validation and manual accumulators
Return a dictionary containing:
- valid_distances
- rejected_rows
- total_miles

Test:
- Mixed valid and invalid data
- Empty dataset
- Original CSV unchanged
### Day 8 — Data Quality Report

The function `create_quality_report()` analyzes a dataset audit and produces a data quality summary.

It:
- Counts valid and rejected rows.
- Calculates the total number of records.
- Calculates the percentage of valid records.
- Calculates the average valid distance.
- Handles empty datasets.
- Returns the results as a dictionary without modifying the original input.

**Tests performed:**
- Normal dataset
- Empty dataset
- Original input remains unchanged
  
## Day_09_function_evaluate_data_quality()

_ The function check wheter a dataset passes a quality threshold
_ Test five different datasets
1- Test a dataset with a quality_percentage less than the threshold and return "REJECT"
2- Test a dataset with exactly the threshold and return "PASS"
3- Test a dataset containing 0 rows and return "EMPTY"
4- Test a dataset with a custom threshold and return "pASS"
5- verify the original dictionary remains unchanged
