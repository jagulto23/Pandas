Project Purpose

The purpose of this project is to analyze the Iris dataset by combining petal and sepal measurement data into a single structured dataset and performing statistical analysis. The project calculates correlations between variables, as well as the mean, median, and standard deviation for each measurement. It also compares iris species to determine which are most and least similar based on quantitative evidence.
This project demonstrates data merging, statistical computation, and basic data analysis using Python and Pandas.

Project Design and Implementation
The project is designed around a structured data analysis workflow:
Load datasets from CSV files
Clean unnecessary columns
Merge datasets into a unified DataFrame
Perform statistical calculations
Analyze and interpret species similarity
The program ensures that petal and sepal measurements are correctly matched using sample_id and species to maintain data integrity.

Class Design
If implemented using a class-based structure, the main class (for example, IrisAnalysis) is responsible for managing data and performing statistical operations.

Class Attributes
petal_data
Stores the DataFrame containing petal measurements.
sepal_data
Stores the DataFrame containing sepal measurements.
iris
The merged DataFrame containing:
sample_id, species, petal_length, petal_width, sepal_length, andsepal_width

Class Methods
load_data()
Reads the CSV files into Pandas DataFrames.
clean_data()
Removes unnecessary columns such as Unnamed: 0.
merge_data()
Merges petal and sepal datasets using sample_id and species.
calculate_correlation()
Computes correlations between the four numeric variables (6 comparisons).
calculate_mean()
Returns the average of each measurement variable.
calculate_median()
Returns the median of each measurement variable.
calculate_std()
Returns the standard deviation of each measurement variable.
compare_species()
Groups the dataset by species and calculates average measurements to determine similarity.

Statistical Analysis
The project calculates:
6 pairwise correlations between:
Petal length
Petal width
Sepal length
Sepal width
Mean of each variable
Median of each variable
Standard deviation of each variable
Species similarity is determined by comparing average measurement values.

Limitations
The analysis assumes clean and complete data.
Missing values are not handled in advanced ways.
The similarity comparison is based on basic statistical measures and does not include clustering or machine learning techniques.
Visualization is not included in the current implementation.

Technologies Used
Python
Pandas
