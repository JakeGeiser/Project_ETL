# ETL Project
### Extract, Transform, and Load datasets into one large clean data set. Project in Dataviz class.


## Group: Carlie Azar, Dave Moorman, Jake Geiser, Andrea Pappa

## Extract 
### I. Sources:
#### A. https://www.kaggle.com/blitzr/movehub-city-rankings?select=cities.csv
#### B. https://www.kaggle.com/blitzr/movehub-city-rankings?select=movehubcostofliving.csv
#### C. https://www.kaggle.com/blitzr/movehub-city-rankings?select=movehubqualityoflife.csv
#### D. https://worldpopulationreview.com/world-cities

### II. Purpose
We extracted 3 CSVs from Kaggle examining an expanse of cities around the world, their cost of living, and quality of life. We also got populations and population densities for the top 1147 cities from worldpopulationreview. Using ETL methodology, we will be investigating municipalities where the population exceeds 500,000. After extracting data from the CSVs, we will reconstruct our findings and reload them into a relational database.  

## Transform 
Using Pandas Python module, we merged the four csv files in the following order: mh_costofliving.csv --> mh_qualityoflife.csv --> mh_cities.csv --> Populations.csv. This order was chosen as the first merge resulted in no loss of rows, but the second resulted in a one to many scenario where we then chose to remove any city that whas repeated. The third and final merge resulted in only keeping the cities with more than 500,000 in population.

## Load 
Added 4 panda Dataframes into PostgreSQL as tables in one database for ease of use later.

