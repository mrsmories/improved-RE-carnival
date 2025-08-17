# Real Estate Data 2001-2022

## Description
This project looks at a large set of real estate sales data gathered from 2001–2022 from 170 different towns primarily in the American Northeast region.  

The data frame has **14 columns and 1,097,629 rows**.  
The goal of this data analysis is to identify any noticeable long-term market trends for this region and compare the markets between different towns.  

My main goal is to practice analysis using Python and Pandas, but I was also attracted to this dataset having a background in real estate. I liked that it is a fairly large dataset spanning such a long time period.  

The questions driving this analysis revolve around:
- Sales by year  
- Sales by town  
- Sale trends for specific towns over time  

## Technologies
- **Python** (Data analysis and visualization)  
- **Libraries**: Pandas (Data manipulation), NumPy (Numerical computing), Matplotlib/Seaborn (Data visualization)  

## Dataset
The data is available for download on Kaggle:  
[Real Estate Dataset](https://www.kaggle.com/datasets/omniamahmoudsaeed/real-estate-sales-2001-2022/data)  

- File size: **125.15 MB**  
- Note: You may need to create a free Kaggle account to access the data.  

## Columns
1. **Serial Number** – A unique identifier for each property record.  
2. **List Year** – The year when the property was listed for sale.  
3. **Date Recorded** – The date the property sale was recorded in the dataset.  
4. **Town** – The town or city where the property is located.  
5. **Address** – The street address of the property.  
6. **Assessed Value** – The value assigned to the property for tax purposes.  
7. **Sale Amount** – The final sale price of the property.  
8. **Sales Ratio** – A ratio of the sale amount to the assessed value, indicating how close the sale price is to the assessed value.  
9. **Property Type** – The type of property (e.g., Residential, Commercial).  
10. **Residential Type** – The specific type of residential property (e.g., Single Family).  
11. **Non Use Code** – Code indicating properties that may not be used for typical purposes (e.g., vacant land).  
12. **Assessor Remarks** – Additional remarks from the assessor about the property.  
13. **OPM Remarks** – Remarks from the Office of Property Management.  
14. **Location** – Geographical coordinates of the property (latitude and longitude).  

## Project Structure
This project has **3 Jupyter notebooks** where the data manipulation is divided into chunks. The work in those notebooks also produces 3 CSV files containing reorganized and filtered data for export into tools like Tableau for further visualization.

1. **RE_import_sales_ratio.ipynb**  
   - Builds the initial data import  
   - Examines overall structure (size & completeness)  
   - Converts 4 columns into categories for processing  
   - Plots missing values  
   - Performs data cleaning for Sale Ratio values  
   - Identifies outliers (low-dollar “non–arm’s length” sales skewing Sale Ratios)  

2. **Sum_by_town.ipynb**  
   - Groups sales by year → plots sales sum by year  
   - Groups data by town → enables comparisons between towns  
   - Provides an example town analysis (Avon)  

3. **Price_levels.ipynb**  
   - Establishes price levels for each sale:  
     - Under $300k  
     - Mid  
     - $700k–$1M  
     - Luxury  
   - Compares number of sales by year, town, region, and sales ratio.  

