# Cleaning and Preparing The Flights Delay Dataset for Model Prediction
The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics tracks the on-time performance of domestic flights operated by large air carriers. Summary information on the number of on-time, delayed, canceled, and diverted flights is published in DOT's monthly Air Travel Consumer Report and in this dataset of 2015 flight delays and cancellations.

​Using flight delay and cancellation data collected and published by DOT's Bureau of Transportation Statistics, which I downloaded via the Kaggle public dataset. I tried to clean and prepare the data for training machine learning model prediction of flight delay reasons using python.


## Issues Found in Data
- **Missing values**- There are some columns that have a large number of zero values. We need to analyze whether the column is intentionally left blank or there is an error in the inputting process. For example, the CANCELLATION_REASON column has 5,729,195 empty rows, indicating that the number of flights that were not canceled. Whereas, the AIR_SYSTEM_DELAY, SECURITY_DELAY, AIRLINE_DELAY, LATE_AIRCRAFT_DELAY, and WEATHER_DELAY columns have 4,755,640 null rows, indicating that the number of flights did not experience delays caused by air system, security, airline, late aircraft, or weather. But we need to ensure the reason why they are null.


## Tools Used
For the data cleaning project, the following tools and libraries were used:
- **Python** for data cleaning tasks.
- **Pandas Library** for instrumental in data manipulation, cleaning and handling missing values.
- **NumPy Library** for utilized for mathematical operations and array handling during the cleaning process.
- **Jupyter Notebooks** provided an interactive environment for code development, exploration and documentation.


## Data Cleaning and Preparing Process
The data cleansing process involves the following steps:
1. **Data Understanding** - The data set is thoroughly examined to understand its structure, fields, and meaning.
2. **Data Exploration** - Exploratory Data Analysis is performed to gain insights into the data, identify patterns, and uncover anomalies.
3. **Handling Missing Values**- Through the EDA conducted, I quickly realized that there were valid reasons for the missing values in the 'ARRIVAL_DELAY' column and a few other columns.
4. **Model Training Preparation** - Ensuring that the data used to train the model (features as well as target variables) has been processed and adjusted in an optimal way to support the learning process of the machine learning model. I used features related to delay reasons, such as 'YEAR', 'MONTH', 'DAY', 'DAY_OF_WEEK', 'AIRLINE', 'SCHEDULED_DEPARTURE', and 'DELAY_REASON'.
5. **Validation and Quality Checks** - The cleaned dataset undergoes rigorous validation to ensure data quality, accuracy, and integrity.
