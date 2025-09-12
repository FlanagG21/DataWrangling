[Housing Prices Data Set from Kaggle](https://www.kaggle.com/datasets/codeinstitute/housing-prices-data)

Package dependencies:
- numpy for numpy objects
- pandas for dataframes and data manipulation
- matplotlib for charts and graphs
- seaborn for charts and graphs
- OS
- google.files 



Jared Schlak: Handled missing data for 10 different columns.  Looked at the data set to view the different categorical and numerical data.  Filled in several different missing values with appropriate values, for example if there was no square footage for a basement or a garage then I could safely assume that their was no garage or basement.  On some of the other data values I filled with a ratio or the mode depending on the situation.  For some of the other columns I was able to do some conditional fills based on other categories.  For example if the Overall Quality Finish of the house was ranked high, then I made an assumption that the GargeFinish would also be high.  Lastly for the missing values of the year the garage was built, I used the same values as the house being built.  Of course this is not perfect, but is a safer assumption than putting in 0 for the year being built or leaving it blank.  

Galen Flanagan: Handled exploratory data analysis. Created heatmap for all numerical values, and finding relationships between floor and basement sizes. Also analyzed the mean and median of sales prices, and how overall house quality effected sales prices. Utilized seaborn for graphs.
