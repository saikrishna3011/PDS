This project aims to analyze a dataset of used cars and identify key factors that influence their prices. The primary objective is to clean, preprocess, and explore the data to uncover meaningful insights, ultimately preparing the dataset for further analysis or predictive modeling.
Dataset

The dataset contains various details about used cars, including:
Make and model of the car
Location of sale
Year of manufacture
Mileage
Odometer (kilometers driven)
Fuel type (petrol or diesel)
Transmission type (manual or automatic)
Number of owners
Engine displacement
Engine horsepower
Number of seats
Price when the car was new
The target variable is the price of each used car, which is given in lakhs (Indian currency).

Steps and Justifications
1. Data Cleaning
Handling Missing Values: We identified missing values in several columns and used different imputation methods based on the data type and distribution:
Mileage: Replaced missing values with the mean.
Engine: Replaced missing values with the median.
Fuel_Type: Replaced missing values with the mode.
Justification: Imputation preserves data integrity without discarding rows, which would result in a loss of valuable information.
2. Data Transformation
Removing Units: Converted columns like Mileage, Engine, and Power to numeric values by removing units (kmpl, CC, bhp). This allowed us to handle and analyze these variables numerically.
Encoding Categorical Variables: Converted Fuel_Type and Transmission columns into one-hot encoded variables to prepare them for machine learning algorithms.
Adding New Features: Created a Car_Age column to represent each car’s age, calculated by subtracting the Year of manufacture from the current year.
3. Exploratory Data Analysis
Selected specific columns to analyze, filtered for high-mileage cars, and examined the distribution of prices across fuel types and other key metrics.
Summarized average car prices based on the fuel type and sorted by car age to gain insights into the factors that may influence a car’s resale price.
