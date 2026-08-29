# eCommerce_Apparel
# E-Commerce Apparel Data Cleaning Project

## Project Overview

This project focuses on cleaning and preparing an e-commerce apparel dataset for future analysis and visualization.

The original dataset contains **25,000+ records** with various data quality issues, including inconsistent formatting, typos, duplicate values, invalid dates, inconsistent category names, and missing values.

The data cleaning process was performed using **Google Sheets** to improve data consistency and prepare the dataset for the next stage of the project.

> This repository currently focuses on the data cleaning process. Data analysis and visualization will be developed in a later stage.

---

## Dataset

The dataset contains e-commerce order-level data with information related to:

* Orders
* Customers
* Customer type
* Geographic information
* Marketing channels and campaigns
* Devices
* Products and categories
* Sales and revenue
* Discounts
* Returns
* Costs and profitability
* Delivery information

The dataset contains approximately **25,000 records** and multiple columns covering customer, product, marketing, sales, and operational data.

---

## Tools Used

* **Google Sheets** — Data cleaning and transformation
* **GitHub** — Project documentation and version control

---

## Data Cleaning Process

The dataset contained several data quality issues that needed to be reviewed and cleaned.

### 1. Customer Data

Issues identified:

* Inconsistent customer type values
* `"New"` and `"New Customer"` represented the same customer type
* `"Repeat"` and `"Returning"` represented the same customer type
* Invalid and inconsistent customer signup dates

Cleaning actions:

* Standardized `"New"` to `"New Customer"`
* Standardized `"Repeat"` to `"Returning"`
* Converted valid customer signup dates into a consistent date format
* Kept unknown or invalid dates unchanged when there was insufficient information to correct them

---

### 2. Geographic Data

Issues identified in:

* Country
* Region
* City

The dataset contained:

* Typos
* Inconsistent capitalization
* Extra spaces
* Different naming formats

Cleaning actions:

* Standardized country names
* Corrected region naming and formatting
* Standardized city names and corrected formatting inconsistencies

---

### 3. Marketing Data

The following columns contained inconsistent values:

* Channel
* Campaign

Examples of issues included:

* Typos
* Inconsistent naming
* Formatting differences
* Spacing inconsistencies

Cleaning actions:

* Standardized values into consistent naming formats
* Corrected known typos and formatting issues

---

### 4. Device Data

The device column contained inconsistent values caused by:

* Different capitalization
* Naming variations
* Formatting inconsistencies

Cleaning actions:

* Standardized device names into consistent categories

---

### 5. Product Data

Data quality issues were identified in:

* Category
* Product name
* Color
* Size

The dataset contained:

* Typos
* Inconsistent capitalization
* Formatting differences
* Missing size values

Cleaning actions:

* Standardized category names
* Corrected product name inconsistencies
* Standardized color values
* Replaced missing size values with `"Unknown"`

---

### 6. Date Data

Issues identified:

* Dates stored as text
* Mixed date formats
* Invalid date values
* Unknown dates

Cleaning actions:

* Converted valid dates into a consistent date format
* Kept invalid or unknown values when there was insufficient information to accurately correct them

---

### 7. Quantity Data

The dataset contained:

* Zero quantity values
* Negative quantity values

A total of approximately **45 records** contained quantities of `0` or `-1`.

These values were retained because there was insufficient information to determine whether they represented data errors, cancellations, adjustments, or other business scenarios.

---

### 8. Financial Data

Issues identified:

* Price formatting inconsistencies
* Zero marketing cost values
* Missing or invalid financial values

Cleaning actions:

* Standardized price formatting
* Retained zero marketing cost values because there was not enough information available to accurately replace them

---

### 9. Delivery Data

The delivery-related data contained:

* Zero values
* Text-based values
* Invalid or inconsistent formatting

Some values were retained when there was insufficient information available to determine the correct value.

---

## Data Quality Decisions

Not all problematic values were automatically modified or removed.

Some records were intentionally retained when there was insufficient information to determine the correct value. This approach helps avoid introducing assumptions or inaccurate information into the dataset.

Examples include:

* Unknown dates
* Zero or negative quantities
* Zero marketing costs
* Invalid delivery values

All identified issues and cleaning decisions were documented during the cleaning process.

---

## Project Structure

```text
├── data/
│   └── Original and cleaned dataset
│
├── documentation/
│   ├── Data dictionary
│   └── Issue log
│
└── README.md
```

---

## Key Learning Objectives

Through this project, I practiced:

* Data cleaning using Google Sheets
* Identifying data quality issues
* Standardizing inconsistent categorical values
* Handling missing and invalid data
* Documenting data cleaning decisions
* Understanding when data should be corrected versus retained
* Preparing raw data for future analysis and visualization

---

## Current Project Status

### Completed

* [x] Data quality assessment
* [x] Data cleaning
* [x] Data standardization
* [x] Issue documentation
* [x] Data dictionary documentation

### In Progress

* [ ] Exploratory data analysis
* [ ] Business insights
* [ ] Data visualization
* [ ] Dashboard development


