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
  
## Day_09_Data_Quality_Gate

_ The function check wheter a dataset passes a quality threshold
_ Test five different datasets
1- Test a dataset with a quality_percentage less than the threshold and return "REJECT"
2- Test a dataset with exactly the threshold and return "PASS"
3- Test a dataset containing 0 rows and return "EMPTY"
4- Test a dataset with a custom threshold and return "pASS"
5- verify the original dictionary remains unchanged

## Day_10_Duplicate_Detection

- The function find_duplication(records) creates two lists seen and duplicates
- seen stores each unique value encountered while looping through the records.
- duplicates stores values that appear again, but each duplicate is added only once. into duplicates

## Day 11 — Data Cleaning Pipeline

### Function: `clean_delivery_pipeline(records)`

**Purpose:** This function cleans delivery records, removes duplicate values, and returns a summary report.

### How the function works

1. The function creates two empty lists: `cleaned_records` and `duplicates`. It also initializes `rejected_count` to zero.
2. It uses a `for` loop to process each record.
3. It replaces commas with periods and uses `float()` to convert records into numbers.
4. If a record cannot be converted or its value is less than or equal to zero, the function counts it as rejected.
5. If a valid value already exists in `cleaned_records`, the function adds it to `duplicates` only if it has not already been recorded there.
6. Otherwise, the function adds the new valid value to `cleaned_records`.
7. Finally, it returns a dictionary containing the cleaned records, duplicate values, and rejected count.

### Testing

I tested the function using valid values, invalid values, repeated duplicates, and an empty list. I also verified that the original list remains unchanged after calling the function.

### What I learned

I learned how to combine loops, conditionals, exception handling, and lists into one data-cleaning pipeline. I also learned that a nested `if` statement helps prevent repeated duplicates from being added more than once.

## Day 12 — Regression Tests

### Purpose

We run regression tests on the `clean_delivery_pipeline()` function to verify that it handles different types of records correctly and that previously fixed bugs do not return.

### Tests Performed

- **Test 1:** Test a list containing four repeated values.
- **Test 2:** Test a list containing duplicate values.
- **Test 3:** Test an empty dataset.
- **Test 4:** Test a list containing invalid values.
- **Test 5:** Verify that the original input list remains unchanged after calling the function.

### Results

All five test scenarios passed successfully.
### What I Learned

I learned how to identify and fix a bug using a nested `if` statement. I also learned why regression tests are important: they help us verify that previously fixed bugs do not return when we modify our code.

## Day 13 — Data Quality Visualization

The `visualize_data_quality(report)` function extracts information from a report dictionary and displays it using a Matplotlib bar chart.

### What the function does

- Displays three bars representing cleaned records, duplicate values, and rejected records.
- Shows the category names on the X-axis and their corresponding counts on the Y-axis.
- Uses the report dictionary to determine the height of each bar.

### Testing

- Tested whether the function displays the correct counts.
- Tested whether an empty dataset can be visualized without raising an error.
- Verified that the original report dictionary remains unchanged after calling the function.

### What I learned

I learned how to use Matplotlib to visualize data quality and how to test a visualization function with different datasets.

## Day 14 — Data Quality Summary

### Purpose
The `summarize_data_quality()` function generates a summary of the quality of a delivery dataset.

### Inputs
The function accepts two parameters:
- `records`: The original list of delivery records.
- `report`: A dictionary returned by `clean_delivery_pipeline()`.

### Process
The function:
1. Counts the total number of records.
2. Counts the unique cleaned records.
3. Retrieves the number of rejected records.
4. Counts the unique duplicate values.
5. Calculates the quality percentage.
6. Handles an empty dataset to prevent division by zero.

### Output
The function returns a new dictionary containing `total_records`, `cleaned_count`, `rejected_count`, `duplicate_count`, and `quality_percentage`.

### Testing
The function was tested with a delivery dataset containing valid, invalid, and duplicate records. Additional tests will verify empty inputs and ensure that the original data remains unchanged.

### What I Learned
I practiced working with dictionaries, function parameters, counting records with `len()`, calculating percentages, and handling division by zero.
