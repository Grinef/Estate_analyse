# Project: Exploratory Data Analysis
### Project Overview

Analyze a dataset from Yandex Realty containing archived listings of real estate sales in St. Petersburg and neighboring areas. Your task is to determine the market value of properties and identify factors influencing property prices. This will aid in developing an automated system to detect anomalies and fraudulent activities.

### Project Instructions

#### Step 1: Data Opening and Initial Exploration
- Path to file: `/datasets/real_estate_data.csv`
- Load the data into a pandas dataframe.
- Review general information using `info()` and `describe()`.
- Construct a histogram for all numerical columns on a single plot.

#### Step 2: Data Preprocessing
- Identify and handle missing values:
  - Determine columns with missing values.
  - Replace missing values where possible (e.g., assume zero balconies if not specified).
  - Document reasons for missing data.
  
- Assess data types:
  - Identify columns needing type conversion.
  - Convert data types as necessary (e.g., dates).

- Address implicit duplicates in the 'locality_name' column.
  - Normalize names to remove inconsistencies.

#### Step 3: Feature Engineering
- Introduce new columns:
  - Price per square meter.
  - Day of the week, month, and year of listing.
  - Floor type (first, last, other).
  - Distance to city center in kilometers (converted from meters).

#### Step 4: Exploratory Data Analysis
- Analyze key parameters:
  - Total area, living area, kitchen area, price, number of rooms, ceiling height, floor type, total floors, distance to city center, distance to nearest park.

- Investigate outliers and anomalies:
  - Clean data where appropriate or remove outliers affecting analysis.

- Examine days on market ('days_exposition'):
  - Build a histogram.
  - Calculate mean and median.
  - Interpret timeframes for typical and atypical sale durations.

- Determine factors influencing total price:
  - Assess correlations with parameters such as area dimensions, room count, floor type, and listing dates.

- Visualize dependencies:
  - Construct graphs to illustrate price dependencies on aforementioned parameters using pivot tables if needed.

- Compute average square meter prices in top 10 localities by listing count.
  - Generate a pivot table detailing average prices and listing counts.
  - Highlight localities with highest and lowest square meter prices.

- Analyze price variations by distance from St. Petersburg city center.
  - Plot average price changes per kilometer radius from the city center.

#### Step 5: Conclusion
- Summarize findings from the analysis.
- Document the outcomes and conclusions drawn from your research.
