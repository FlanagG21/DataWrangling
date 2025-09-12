
### Project Title
Homework #3: Collaborative Data Wrangling & EDA
DSE 511 – Fall 2025

### Dataset Information

Source: [Housing Prices Data Set from Kaggle](https://www.kaggle.com/datasets/codeinstitute/housing-prices-data)

Date accessed: [09/12/2025]

Description: This data set is called House Prices.  It consists of 24 columns and has 1460 rows. It includes columns such as SquareFoot for 1st and 2nd floor, Basement SqFt, GarageArea, Number of Bedrooms, Year Built, Condition, and finally price. This data set would be good to try to predict house prices for this specific area, given the different attributes.  There was missing data in 10 of the 24 columns, that we would have to figure out what to do.  Overall, this was a pretty manageable data set.

Size: 24 columns x 1460 rows.  138 kB.

License (if known): Kaggle Dataset - public data set

### Methods

Data Cleaning (Jared Schlak)

Handled missing data for 10 different columns.  Looked at the data set to view the different categorical and numerical data.  Filled in several different missing values with appropriate values, for example if there was no square footage for a basement or a garage then I could safely assume that their was no garage or basement.  On some of the other data values I filled with a ratio or the mode depending on the situation.  For some of the other columns I was able to do some conditional fills based on other categories.  For example if the Overall Quality Finish of the house was ranked high, then I made an assumption that the GargeFinish would also be high.  Lastly for the missing values of the year the garage was built, I used the same values as the house being built.  Of course this is not perfect, but is a safer assumption than putting in 0 for the year being built or leaving it blank. There were some columns that we kept in the dataset, but did not use much in the EDA due to relevance to the price.  

Tools/libraries used (e.g., pandas, numpy).
- numpy for numpy objects
- pandas for dataframes and data manipulation
- matplotlib for charts and graphs
- seaborn for charts and graphs
- OS
- google.files 

Exploratory Data Analysis (Galen Flanagan)

1st we Created a heatmap for correlation for all numerical values.
Then we graphed the relationship between floor and basement sizes. (1st and basement and 1st and 2nd). In addition we checked the relationship between the 1st floor and the 2nd floor for houses where the second floor was non-zero.
In addition we printed the correlation values for all three of these values (1st floor, 2nd floor and basement square feet) for both non-zero and all houses to spot differences. 
Then we checked the median and mean of sale prices. In addition we plotted histograms of sale price and overall quality. lastly we made a violin plot of sale price based on overall quality to spot how overall quality effected sale price.

### Results

 It was found that 1st floor size correlated very strongly and was nearly one to one with basement size. It was also found that 2nd floor when it existed correlated with the size of the 1st floor but the was more variation

 We also found that sale price was a right skewed distribution based off its median being lower than its mean and that the overall quality had a strong effect on the sale price

Optional: brief reflection on what was interesting or unexpected.

I did not expect the lower corelation between the size of the second floor and the first floor relative to the correlation between the 1st floor and the basement. I had initially expected it to be roughly equal because floor sizes are generally about the same on every level in my experience.

### Collaboration Notes

Jared Schlak: Did the Data Cleaning

Galen Flanagan: Did the EDA and visulization

Both: Readme documentation and merge conflict resolution

### Reproducibility Instructions

open in google colab and hit run, starting with DataCleaningProject.ipnyb for cleaning and then the EDA.ipnyb for visualization. Do not forget to upload the data files into the documents to run them. (You can also skip to the EDA.ipnyb by using cleaned_house_data.csv instead of house_prices_records.csv)

Dependencies (e.g., requirements.txt or conda environment).

google colab packages are used

### Merge Conflict Reflection (Required)

Merge conflict occurred because both members edited the readme at the same time. The merge conflict was easily resolved by taking everything from the more complete version of the readme. (Take all changes from the right in VS code)




 

