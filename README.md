# nosql-challenge

# Overview of Project 

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. I had been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

# Purpose 
Use Non-SQL databases to access and create edit using MongoDB and pyMongo. 

# Requirements 
Pandas, Juptyer Notebook, MongoDB, pymongo. 

# Database Set-up 
1. Import the data from the establishments.json file and name the database uk_food and the collection establishments. 
2. Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).
3. Create an instance of the Mongo Client.
4. Confirm that you created the database and loaded the data properly:
5. List the databases you have in MongoDB. Confirm that uk_food is listed.
6. List the collection(s) in the database to ensure that establishments is there.
7. Find and display one document in the establishments collection using find_one and display with pprint.
8. Assign the establishments collection to a variable to prepare the collection for use.

# Update the Database 

The magazine editors have some requested modifications for the database beforeany queries or analysis for can be performed. Make the following changes to the establishments collection:
1. An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis.
2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3. Update the new restaurant with the BusinessTypeID you found.
4. The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
5. Some of the number values are stored as strings, when they should be stored as numbers. Use update_many to convert latitude and longitude to decimal numbers.

# Exploratory Data Analysis 
Answer the following questions for Eat, Pray, Love Magazine: 

1. Which establishments have a hygiene score equal to 20?
41. Please see "NoSQL-analysis.ipynb" for details. 

2. Which establishments in London have a RatingValue greater than or equal to 4?
34. Please see "NoSQL-analysis.ipynb" for details. 

3. What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
Please see "NoSQL-analysis.ipynb" for details. 

4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
55. Please see "NoSQL-analysis.ipynb" for details. 

# Credits 
Data accessed from UK Food Standards Agency Links to an external site.(2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GB Links to an external site.. Contains public sector information licensed under the Open Government Licence v3.0 by the University of Toronto School of Continuing Studies in partnership with edX Boot Camps LLC for educational purposes only.  
