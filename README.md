                                                 #**NETFLIX MOVIES ANALYSIS**
                                                     
##**1.Project Overview **
    
    
    This project analyse Netflix movies dataset collected from Kaggle.com. 
    
    
    The goal is to derive insights into thew trends and patterns in Netflix’s catalogue to guide strategic business decisions.
    
##**2.Dataset Summary **
 
  Rows: 16000
  
  Columns: 13 
 
  *Key Features:*
   
     •	Netflix Columns( Show_id, Type, Title, Director, Country, Date_added, Rating, Genres, Language, Popularity, Vote_Count, Vote_Average, Revenue.
    
     •	Missing Data: 705 values in Review Director, Country, Genres column.
 
##**3.Exploratory Data Analysis using Python**
 We began with data preparation and cleaning in Python: 
 
    ###● Data Loading:
          Imported the dataset using pandas. 
    ###● Initial Exploration:
         Used df.info() to check structure and df.describe() for summary statistics.
    ###● Missing Data Handling: 
         Checked for null values and imputed missing values in the Review Director, Country, Genres column using df.dropna(inplace=True)
    ###● Column Standardization:
         Renamed columns to snake case for better readability and documentation. 
    ###● Data Consistency Check:
          Verified if
              	df[['TITLE','DIRECTOR']].head(10)
              	df[['COUNTRY','RATING']].head(10)
    ###● Database Integration:
          Connected Python script to PostgreSQL and loaded the cleaned DataFrame into the database for SQL analysis.


##**4. Data Analysis using SQL (Business Transactions)**
         We performed structured analysis in PostgreSQL to answer key business questions: 

     1.	Top 5 Titles by Revenue – Found titles with the highest average revenue.
    
     2.	Top 3 Country-Found most use movie count of countries.

     3.Action vs Drama Movies-Compared average revenue across movies status.

     4.Highest Movies User Engagement-Found titles on the high vote_count.

     5.High use of Language-Identify to language with the highest popularity to use them.

     6.Top 5 Directors by Ratings- Found directors with the highest average review ratings.

     7.2019 vs 2020 Movies Revenue-Identified movies in 2019 and 2020 total revenue with the date_added.

     8. Ratings by Country-identified the country is at least 50 movies ratings.

##**5. Dashboard in Excel**
       
         Finally, we built an interactive dashboard in Excel to present insights visually. 
             
              	Connect the data in SQL from Excel Sheet.

 
