# CGM Data Project  

This project automates the processing and visualization of continuous glucose monitor (CGM) data. It uses Python and SQLite to create and maintain a database of readings, ensuring clean, consistent data for analysis.  

The program:  
- Detects the latest CSV file of glucose readings without manual renaming or file moves  
- Validates data integrity by removing duplicates and checking for missing dates  
- Restricts stored readings to the most recent 90 days, optimizing storage and relevance  
- Exports the cleaned dataset for use in Tableau visualizations  

## Repository Contents  
- **Create Database SQL Magic.ipynb**  
  Jupyter Notebook for creating an SQLite database, adding a table, and inserting records.  

- **Dexcom Clarity Readings v3.ipynb**  
  Python code that locates the newest data file in the downloads folder, processes it, and updates the SQLite database. Manual file handling is no longer required.  

- **Guide to Continuous Glucose Monitor Visualizations.pdf**  
  A reference guide describing the visualization styles, analytical approaches, and commonly used CGM measures.  

## Visualizations  
Explore the interactive Tableau dashboards here:  
[Tableau Public – CGM Data](https://public.tableau.com/views/CGMData/ContinuousGlucoseMonitorCGMData?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  

## Related Series  
**Working with CGM Data: Python, SQLite, and Tableau in a 4-Part Series**  
[Read the series here](https://jcsanalytics.com/index.php/working-with-cgm-data-python-sqlite-and-tableau-in-a-4-part-series)  

## Project-Specific Extensions: Hourly Analysis
**Guide to TIR and CV Visualizations (PDF)**  
This guide documents project-specific hourly visualizations that extend standard CGM reporting. It explains why daily summaries can obscure timing-related patterns and how hour-by-hour Time in Range and Coefficient of Variation views reveal consistent structure when multiple days are examined together. These visualizations are exploratory and are not part of standardized CGM reporting.  
[Explore the Example Hourly Time in Range Example Visualizations at Tableau Public](https://public.tableau.com/views/ExampleTIRVisualizations/ExampleTimeinRangeandCoefficientofVariationCVVisualizations?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

For more on the patient-centered side of this approach:  
[How an Hour-by-Hour View Transforms Time in Range Insights](https://jcst2d.com/index.php/articles/how-an-hour-by-hour-view-transforms-time-in-range-insights)
