#Real Estate Data 2001-2022
  ##Description:
    This project looks at a large set of real estate sales data gathered from 2001-2022 from 170 different towns primarily in the American NorthEast region.
The data frame has 14 columns and 1,097,629 rows.  The goal of this data analysis is to identify any noticable long term market trends for this region and compare the     markets between different towns in the region.  My main goal is to practice analysis using Python and pandas, but I was also attracted to this dataset having a background in real estate.  I liked that it is a fairly large dataset over such a long time period.  The questions driving this analysis revolve around sales by year and sales by town so that sale trends can be observed over time, by town and per specific town over time.
  ###Technologies:
Python (Data analysis and visualization) Libraries: Pandas (Data manipulation), NumPy (Numerical computing), Matplotlib/Seaborn (Data visualization)
  ###Dataset:
    The data is available for download on Kaggle.
    [Real Estate Dataset](https://www.kaggle.com/datasets/omniamahmoudsaeed/real-estate-sales-2001-2022/data)
    The csv is 125.15 MB  Please note that you may have to create a free Kaggle account to access the data.
  ###Columns:
    1-Serial Number: A unique identifier for each property record.
    2-List Year: The year when the property was listed for sale.
    3-Date Recorded: The date the property sale was recorded in the dataset.
    4-Town: The town or city where the property is located.
    5-Address: The street address of the property.
    6-Assessed Value: The value assigned to the property for tax purposes.
    7-Sale Amount: The final sale price of the property.
    8-Sales Ratio: A ratio of the sale amount to the assessed value, potentially indicating how close the sale price is to the assessed value.
    9-Property Type: The type of property (e.g., Residential, Commercial).
    10-Residential Type: The specific type of residential property, such as Single Family.
    11-Non Use Code: Code indicating properties that may not be used for typical purposes (e.g., vacant land).
    12-Assessor Remarks: Additional remarks from the assessor about the property.
    13-OPM Remarks: Remarks from the Office of Property Management.
    14-Location: Geographical coordinates of the property (latitude and longitude).
  ###Project Structure
    The project has 3 Jupyter notebooks where the data manipulation is divided into 3 chunks.  Also the work in those notebooks lead me to create 3 csv files containing reorganized and filtered sections of the data for export into other programs such as Tableau for further visualization creation.
    1. RE_import_sales_ratio.ipynb : builds the initial data import, ascertains the overall structure of the data looking for size and completeness, 4 columns are turned into categories for easy of processing and missing values are plotted.  There is some data cleaning that is included in the initial import for the sake of the Sale Ratio values.   The remainder of the notebook deals with finding outlier values caused by sales recorded for low dollar amounts representing sales that are not "Arm's Length" sales that highly skew the Sales Ratio data.
    2. Sum_by_town.ipynb :  This notebook first groups the sales by year to get a sales sum by year which is plotted.  Then the notebook groups the data by town so that individual towns can be looked at by year, and compared to each other, by proximity, or other relevent criteria.  The example town Avon is also plotted.
    3. Price_levels.ipynb : The goal of this notebook is to establish price levels for each sale in the dataset so that the number of sales in those levels can be compared by year, town, region, and sales ratio.  The price levels are set at "Under $300k", "Mid", "$700k-$1M", "Luxury".
