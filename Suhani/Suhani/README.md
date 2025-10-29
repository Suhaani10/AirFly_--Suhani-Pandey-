1. Data Understanding

What the dataset represents (e.g., records of passengers and flight details).
The goal — for example: analyzing reasons for flight delays, identifying patterns, or predicting delay probability.
The types of variables present:
Categorical – Gender, Flight Status, Country Name, Airport Continent.
Numerical – Age
Date/Time – Departure Date, Arrival Date.

2. Data Cleaning / Preprocessing Steps
   a. Importing and Inspecting Data
     Load the dataset and inspect the first few rows to understand structure.
     Check the number of rows and columns.
     Check the data types of each column (e.g., object, int, float, datetime).
     Verify column names (remove leading or trailing spaces).

   b. Removing Duplicates and Irrelevant Columns
    Remove duplicate rows to avoid redundancy.
    Drop irrelevant columns that do not contribute to analysis (like passenger ID, personal names, etc.).
    Keep only meaningful columns that relate to flight performance or passenger information.

   c. Handling Missing Values
     Identify missing data in each column.
     Decide how to handle missing values:
     Drop rows with too many missing fields.
     Fill (impute) missing numerical values using the mean or median.
     Fill categorical values with the mode or a placeholder like "Unknown".
     The method chosen depends on how important that column is for analysis.

   d. Feature Engineering
      Create new features that may improve insights:
      Delay flags: “Is Delayed”, “Is Cancelled”.
      Group ages into ranges: “Young”, “Adult”, “Senior”.
      Create “International or Domestic” indicator based on country.

 Exploratory Data Analysis (EDA)

  a. Univariate Analysis
       Study one column at a time.
       Numerical variables: Use histograms or summary statistics (mean, median, mode, range).
       Categorical variables: Use bar charts or pie charts to show frequency distribution.
       Example: Proportion of flights that are “On Time”, “Delayed”, or “Cancelled”.

  b. Bivariate Analysis
         Study the relationship between two variables.
         Compare Flight Status with:
         Age → if older passengers experience more delays.
         Country Name or Airport Continent → which locations have the highest delay rate.

c. Multivariate Analysis
        Study three or more variables together.
        Example: “Delay rate by Month and Continent” or “Gender vs Age group vs Flight Status”.

d. Correlation Analysis
      For numerical variables, calculate correlation coefficients to see how variables relate.
      Display correlations visually using a heatmap.
