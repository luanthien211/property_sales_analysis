# Data Dictionary

Sydney residential property sales dataset (3,000 records). The cleaned student subset used for the descriptive, correlation, and regression sections contains 295 records.

| Column | Type | Description |
|---|---|---|
| Sort ID | Integer | Partition key (0 to 9) used to assign a 295 to 300 row student subset |
| Suburb | Text | Sydney suburb where the property is located |
| Council Area 1 | Text | Local council area, populated with VLOOKUP against the Council Area lookup table |
| Council Area 2 | Text | Local council area, populated with XLOOKUP as a cross check against Council Area 1 |
| Property Type | Text | Apartment, House, Townhouse, or Villa |
| Price | Currency (AUD) | Sale price |
| Bedrooms | Integer | Number of bedrooms |
| Bathrooms | Integer | Number of bathrooms |
| Land Size (sqm) | Integer | Land area in square metres |
| Year Built | Integer | Year of construction |
| Sale Date | Date | Date of sale |
| Inspection Rating | Text | Poor, Average, Good |
| Agent Name | Text | Listing agent |
| Commission Rate (%) | Decimal | Agent commission percentage |
| Council Rate ($/year) | Currency (AUD) | Annual council rate |
| Distance to Nearest Station (km) | Decimal | Distance to the closest train station |
| House Area (sqm) | Integer | Internal floor area in square metres |
| NAPLAN Score of Nearest School | Integer | Standardised test score of the nearest school |

## Cleaning notes
Five rows in the student subset contained invalid entries and were removed before analysis: a negative bedroom count, a placeholder agent value, a non property value in Property Type, a future Year Built, and a zero Land Size. See Question 1 in the report for detail.
