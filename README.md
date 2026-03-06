# data_platform_group_project

## Test weather data (2016-2026) and ETL pipeline for data cleaning 

**Columns**
- date
- avg_temp
- min_temp
- max_temp
- rainfall_mm
- humidity
- weather_notes

 ## Intentional problems in the dataset

 **Missing / inconsistent values**
 - "", NA, None
 - blank weather notes

 **Mixed units**
 - 12.4C
 - 5.6mm

 **Text noise**
 - trace rainfall
 - SUNNY, storm !!!, mixed capitalization

**Invalid values**
- humidity values like 120
- swapped min_temp and max_temp

**Date format inconsistencies**
- YYYY-MM-DD
- DD/MM/YYYY
- MM-DD-YYYY

**Duplicates**
- ~100 duplicated rows


## Cleaning Workflow 
- Parse mixed date formats 
- Convert temperature columns to numeric 
- Strip units (C, mm, %) 
- Fix min/max swapped values 
- Handle missing values 
- Flagging suspicious values 
- Replace impossible values with (e.g, NaN)l
- Remove duplicates 
- Standardize weather_notes text

## Finally : Create a data summary report and then export cleaned data as csv 


