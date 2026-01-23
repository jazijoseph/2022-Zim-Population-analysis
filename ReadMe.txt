

 Zimbabwe 2022 Population Census Analysis

Project Overview

This project is a detailed demographic analysis of the Zimbabwe 2022 Population Census. Driven by a personal goal to work with data from my motherland, I extracted and transformed static PDF reports from the **Zimbabwe National Statistics Agency (ZIMSTAT)** into a clean, analysis-ready dataset. The project explores population distribution, gender ratios, and household density across all 10 provinces and 90 districts of Zimbabwe .

Objectives


Data Accessibility**: Transform tabular PDF data into a structured CSV format for the global data science community .


 
Provincial Analysis: Compare total populations and gender distributions across provinces.


 
Gender Metrics: Calculate and visualize Male-to-Female (M:F) ratios at ward, district, and provincial levels .


 
Household Insights: Analyze the average number of people per household across different regions.



🛠️ Data Extraction & Cleaning (The "Heavy Lifting")

Since official data was only available in PDF format, significant preprocessing was required:

1. 
Conversion: Used SmallPdf to convert tabular PDF pages into Excel.


2. 
Structural Cleaning: Manually joined tables, removed maps/table of contents, and added missing `Province` and `District` headers.


3.Python Processing:
Utilized Pandas to split "messy" overlapped columns where Ward names and population counts were merged .


Cleaned numeric strings by removing commas and handling null values .


Standardized data types for `Male`, `Female`, `Total`, and `Households` .





 Key Insights

National Gender Balance: In all provinces, females outnumber males. The sex ratio ranges from 85.9 (Bulawayo) to 97.5 (Mashonaland West) males per 100 females.



Province Density: Midlands and Manicaland show the highest frequency of districts, while Harare and Bulawayo have fewer districts but higher population density.


 
Household Size: The average household size varies by district, with rural areas like **Beit Rural** averaging ~4.05 people per house compared to **Beit Urban** at ~3.33 .


 
Bulawayo Highlight: Bulawayo has the largest female majority in the country.



 Technical Stack

Language: Python
Libraries: Pandas (Data Manipulation), Matplotlib & Seaborn (Visualization), NumPy
Tools**: SmallPdf (Initial extraction)

 Repository Structure

 `2022_Population_Census.pdf`: The original source document from ZIMSTAT.
 
Cleaned_Population.csv`: The final processed dataset containing 1,961 records.


Zimbabwe_Census_Analysis.ipynb`: The full Jupyter Notebook containing data cleaning and EDA.

---

 💡 Recommendation for Future Work

For others looking to extract similar data, I recommend exploring Python libraries like Camelot or Tabula-py to automate the PDF-to-CSV extraction process directly.

Author: [JAZI JOSEPH DATA SCIENTIST -ZW]


DATE: December 20, 2025