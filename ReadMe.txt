Zimbabwe 2022 Population Census Analysis

Project Description

This project is a comprehensive demographic analysis of the Zimbabwe 2022 Population Census. In pursuit of a personal interest to work with data from my motherland, I processed and transformed static PDF reports from the Zimbabwe National Statistics Agency (ZIMSTAT) into a clean, analysis-ready dataset. The project examines population distribution, gender ratios, and household density for all 10 provinces and 90 districts of Zimbabwe .

Objectives

Data Accessibility: Transform tabular PDF data into a structured CSV format for the global data science community .

Provincial Analysis: Compare total populations and gender distributions across provinces.

Gender Metrics: Calculate and visualize Male-to-Female (M:F) ratios at ward, district, and provincial levels .

Household Insights: Analyze the average number of people per household across different regions.

Data Extraction & Cleaning (The "Heavy Lifting")

As the official data was provided in PDF format only, extensive data cleaning was necessary:

1. Conversion: Employed SmallPdf to convert tabular PDF pages into Excel.

2. Structural Cleaning: Manually merged tables, eliminated maps/table of contents, and included missing `Province` and `District` headers.

3. Python Processing:
   Employed Pandas to split "messy" overlapped columns where Ward names and population figures were combined .

Cleaned numeric strings by removing commas and null values.

Normalized data types for `Male`, `Female`, `Total`, and `Households` .

Key Insights

National Gender Balance: In all provinces, the number of females exceeds that of males. The sex ratio varies from 85.9 (Bulawayo) to 97.5 (Mashonaland West) males per 100 females.

Province Density: Midlands and Manicaland record the highest number of districts, while Harare and Bulawayo record fewer districts but with higher density.

Household Size: The average household size per district varies, with rural districts such as **Beit Rural** averaging ~4.05 people per house compared to **Beit Urban** at ~3.33 .

Bulawayo Highlight: Bulawayo records the highest female majority in the country.

Technical Stack

Language: Python
Libraries: Pandas (Data Manipulation), Matplotlib & Seaborn (Visualization), NumPy
Tools**: SmallPdf (Initial extraction)

Repository Structure

`2022_Population_Census.pdf`: The original source document from ZIMSTAT.

`Cleaned_Population.csv`: The final processed dataset containing 1,961 records.

`Zimbabwe_Census_Analysis.ipynb`: The full Jupyter Notebook containing data cleaning and EDA.

----------------------------------------------------------------------------------------------------

Recommendation for Future Work

For others looking to extract similar data, I recommend exploring Python libraries like Camelot or Tabula-py to automate the PDF-to-CSV extraction process directly.

Author: [JAZI JOSEPH DATA SCIENTIST -ZW]

DATE: December 20, 2025

