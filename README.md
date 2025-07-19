This project involves cleaning a dataset of job listings to prepare it for further analysis or modeling.
Tools used: python (pandas, numpy, seaborn and matplotlib).

Handled Missing Values:
Missing values were treated with context-aware imputation. For example, type, sector, and size columns were filled using either mode or labeled as 'unknown', while rating used the mean.

Cleaned and Standardized Text Columns:
Uniform formatting was applied using some functions to ensure consistent values across categorical columns such as job type, company type, and revenue.

Extracted and Converted Salary Components:
Created new columns for min_salary, max_salary, and average_salary by parsing the original salary estimate field. Hourly salaries (values < 500) were detected and scaled to yearly salary using a 2080-hour work year.

Filtered Outliers Using Histograms:
Outlier removal was done visually and intuitively using histograms instead of the IQR or Z-score method, the data was not complex.
