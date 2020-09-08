# ETL Project
### Extract, Transform, and Load datasets into one large clean data set. Project in Dataviz class.


## Group: Carlie Azar, Dave Moorman, Jake Geiser, Andrea Pappa

## Extract 
### I. Sources:
#### A. https://www.kaggle.com/blitzr/movehub-city-rankings?select=cities.csv
#### B. https://www.kaggle.com/blitzr/movehub-city-rankings?select=movehubcostofliving.csv
#### C. https://www.kaggle.com/blitzr/movehub-city-rankings?select=movehubqualityoflife.csv
#### D. https://worldpopulationreview.com/world-cities

### II. We extracted 3 CSVs from Kaggle examining an expanse of cities around the world, their cost of living, and quality of life. We also got populations and population densities for the top 1147 cities from worldpopulationreview. Using ETL methodology, we will be investigating municipalities where the population exceeds 500,000. After extracting data from the CSVs, we will reconstruct our findings and reload them into a relational database.  

## Transform 
### I. Using Pandas Python module, we merged the four csv files in the following order: mh_costofliving.csv --> mh_qualityoflife.csv --> mh_cities.csv --> Populations.csv. This order 
Python, Pandas, and SQL will be used to clean, filter, and aggregate the data. Using Pandas Python module, we merged the four csv files and removed rows with missing data.  We will also bring in SQLAlchemy as another open-source tool and object relational mapper (ORM).

## Load 
### I. Loading data into a relational database for referencing and analysis

