# Airline Operations Control Daily Report Automation

A Python-based automation system for generating daily Airline Operations Control reports, developed and deployed for operational reporting workflows within an airline's Operations Control Centre (OCC).

## Overview

This project automates the generation of daily airline operational reports from flight performance data.

The system processes the input Excel file, performs data filtering and validation, calculates operational performance indicators, analyses delay information, and automatically generates formatted PDF and Excel reports.

A standalone Windows executable is provided, allowing the reporting workflow to be executed without requiring Python or any additional programming environment.

## Download

[Download Windows Executable](./dist/test2-good.exe)

## Key Features

- Automated processing of airline operational data
- Flight schedule and flown-flight analysis
- On-Time Performance (OTP) calculation
- Load Factor calculation
- Passenger data aggregation
- Cargo / CGO data aggregation
- Delay code analysis
- Departure delay analysis
- Identification of major delays
- Origin and destination airport information
- Automated Excel report generation
- Automated PDF report generation
- Standardised report formatting
- Standalone Windows executable
- Designed for daily OCC reporting workflows

## How to Use

### Windows Executable

The standalone executable is located in the `dist` folder:

- `test2-good.exe`

The executable is designed to automatically read the input file:

- `Performance Report 2026.xlsx`

and generate the following reports:

- `Daily_Operations_Report.pdf`
- `Daily_Operations_Report.xlsx`

### Step 1 — Prepare the Input File

Place the input Excel file in the same folder as the executable:

`Performance Report 2026.xlsx`

The folder should contain:

    dist/
    ├── test2-good.exe
    ├── Performance Report 2026.xlsx
    ├── header.png
    └── ...

### Step 2 — Run the Application

Double-click:

`test2-good.exe`

No Python installation or additional software environment is required.

### Step 3 — Generated Reports

After the executable finishes processing the input data, the following files will be generated automatically in the same directory:

- `Daily_Operations_Report.pdf`
- `Daily_Operations_Report.xlsx`

The workflow can therefore be summarised as:

    Performance Report 2026.xlsx
              ↓
        test2-good.exe
              ↓
    ┌─────────┴─────────┐
    ↓                   ↓
    PDF Report      Excel Report

## Workflow

    Operational Flight Data
            ↓
    Excel Input Processing
            ↓
    Python / Pandas Data Processing
            ↓
    Data Filtering & Validation
            ↓
    Operational KPI Calculation
            ↓
    Delay Code Analysis
            ↓
    Daily Report Generation
            ↓
       ┌────┴────┐
       ↓         ↓
    PDF Report  Excel Report

## Operational Metrics

The automated reporting workflow can generate and analyse operational indicators including:

| Metric | Description |
|---|---|
| Scheduled Flights | Number of scheduled flights |
| Flown Flights | Number of operated flights |
| OTP | On-Time Performance |
| Load Factor | Passenger load factor |
| Passenger Volume | Aggregated passenger volume |
| Cargo Volume | Aggregated cargo volume |
| Delay Minutes | Recorded departure delay duration |
| Delay Codes | Categorisation of operational delays |
| Major Delays | Identification of significant departure delays |
| Origin / Destination | Airport-level flight information |

## Delay Analysis

The system processes operational delay information and categorises delays according to their corresponding delay codes.

This provides a structured basis for analysing operational delay patterns and identifying potential areas for operational improvement.

The reporting workflow can support:

- Delay-code frequency analysis
- Delay-duration analysis
- First-wave flight analysis
- Route-level analysis
- Airport-level analysis
- Daily OTP analysis
- Major departure delay identification
- Recurring operational issue analysis

## Project Structure

    Airline-Operations-Control-Daily-Report-Generator/
    │
    ├── README.md
    │
    └── dist/
        ├── test2-good.exe
        ├── Performance Report 2026.xlsx
        ├── header.png
        ├── Daily_Operations_Report.pdf
        └── Daily_Operations_Report.xlsx

### File Description

| File | Description |
|---|---|
| `test2-good.exe` | Standalone Windows application for automated report generation |
| `Performance Report 2026.xlsx` | Input operational dataset |
| `header.png` | Report header asset |
| `Daily_Operations_Report.pdf` | Automatically generated PDF report |
| `Daily_Operations_Report.xlsx` | Automatically generated Excel report |

## Technology Stack

- Python
- Pandas
- OpenPyXL
- Jupyter Notebook
- ReportLab
- PyInstaller
- Microsoft Excel
- PDF

## Deployment

The system was developed and deployed for use within an airline's Operations Control Centre and is designed around a daily operational reporting workflow.

The standalone executable packages the Python-based reporting workflow into a Windows application, allowing users to generate the required reports without directly interacting with the underlying Python code or environment.

The project demonstrates the application of Python-based automation, data processing, and analytics to an operational aviation environment.

# Data & Confidentiality Disclaimer

## Important Notice

All operational data included in this public repository is fictional, synthetic, anonymised, or otherwise modified specifically for demonstration and portfolio purposes.

The data does not represent actual airline operations and must not be interpreted as actual:

- Flight schedules
- Flight numbers
- Routes
- Passenger volumes
- Cargo volumes
- OTP results
- Delay performance
- Operational KPIs
- Aircraft operations
- OCC activities
- Commercial performance
- Company performance

Any similarity between the demonstration data and real-world airline operations is coincidental.

This repository is intended to demonstrate the technical implementation, data-processing methodology, automation workflow, and reporting capabilities of the project rather than disclose actual airline operational information.

No confidential company information, personal information, passwords, API keys, credentials, or proprietary system access information is intentionally included in this repository.

## Company Confidentiality

The project was developed in an airline operational environment. The public version of this project has been prepared for portfolio and technical demonstration purposes.

Actual company operational data, internal records, confidential information, and proprietary system access information are not intended to be disclosed through this repository.

The datasets and generated reports included in the public version should be treated as demonstration materials only and should not be used to infer actual airline operational performance.

If any file or information is identified as potentially confidential or proprietary, it should not be used, reproduced, or distributed without appropriate authorisation.

## Source Code

The project was originally developed using Python and Jupyter Notebook.

The executable version packages the underlying Python implementation into a standalone Windows application using PyInstaller.

This allows the end user to operate the reporting workflow without requiring access to the development environment.

## Future Development

Potential future improvements include:

- Scheduled automatic report generation
- Automated data ingestion
- Integration with operational databases
- Automated email distribution
- Dashboard-based operational monitoring
- Historical OTP and delay trend analysis
- Automated anomaly detection
- Operational trend monitoring
- Additional KPI monitoring
- Interactive reporting dashboards

## Author

**Jason Zhao**

Aeronautical Engineering  
Python | Data Analytics | Automation | Aviation Operations

## Disclaimer

This repository is provided for educational, portfolio, and technical demonstration purposes.

The public version of this project is not intended to disclose or reproduce confidential airline operational information.

All demonstration data should be treated as fictional and non-representative of actual airline operations.
