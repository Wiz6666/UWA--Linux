# OSTS4407-OSTS Project 2: Incident and Breach Data Analysis

## Overview
This repository contains a series of Bash scripts developed for analyzing incident and breach data as part of the OSTS4407 course. Each script is designed to perform specific data processing and analysis tasks on the YouTube dataset provided by the university coordinator.

## Scripts

### 1. DataPreprocessorCLI
- **Purpose**: Preprocesses input data by checking integrity, handling errors, and augmenting the dataset with additional columns for month and year extracted from date fields.
- **Input**: Path to the input file.
- **Output**: Standard output with enhanced data and error messages redirected to standard error if issues are detected.
- **Usage Example**:
  ```bash
  ./DataPreprocessorCLI input_file.tsv

### 2. IncidentAnalyzerCLI
- **Purpose**: Analyzes incidents to identify the state or year with the maximum number of incidents. It supports queries for the maximum incidents overall, by state, or by year.
- **Input**:Path to the input file and a command specifying the analysis type (maxstate, maxyear, state code, or year).
- **Output**:Prints the result of the analysis to standard output.

- **Usage Example**:
  ```bash
./IncidentAnalyzerCLI input_file.tsv maxstate

### 3. MonthlyBreachAnalysisCLI
- **Purpose**:Analyzes the frequency of breaches per month and calculates the Median Absolute Deviation (MAD) from the median to identify significant deviations.
- **Input**:Path to the input file.
- **Output**:Outputs the median, MAD, and a detailed breakdown of breaches per month along with deviations flagged as significant.
- **Usage Example**:
  ```bash
./MonthlyBreachAnalysisCLI input_file.tsv

###  Requirements
Bash shell; gawk (GNU Awk), especially for MonthlyBreachAnalysisCLI
