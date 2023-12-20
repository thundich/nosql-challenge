# nosql-challenge
Module 12 Challenge

Tamara Hundich

12/19/2023

  Michigan State University edX Data Analytics Bootcamp 

  Challenge 12: MongoDB and NoSQL

## Requirements
  - Part 1:  Database and Jupyter Notebook Set Up
        - Use NoSQL_setup_starter.ipynb for this section of the challenge.
        - Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.
        - Within your notebook, import the libraries you need: PyMongo and Pretty Print (pprint).
        - Create an instance of the Mongo Client.
        - Confirm that you created the database and loaded the data properly:
            - List the databases you have in MongoDB. Confirm that uk_food is listed.
            - List the collection(s) in the database to ensure that establishments is there.
            - Find and display one document in the establishments collection using find_one and display with pprint.
        - Assign the establishments collection to a variable to prepare the collection for use.
  - Part 2:  Update the Database
        - Use NoSQL_setup_starter.ipynb for this section of the challenge
        - The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:
            - An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the databas. 
            - Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
            - Update the new restaurant with the BusinessTypeID you found.
            - The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
            - Some of the number values are stored as strings, when they should be stored as numbers
                - Use update_many to convert latitude and longitude to decimal numbers.
                - Use update_many to convert RatingValue to integer numbers.
  - Part 3: Exploratory Analysis
       - Use NoSQL_analysis_starter.ipynb for this section of the challenge.
       - Use the following questions to explore the database, and find the answers, so you can provide them to the magazine editors.
            - Unless otherwise stated, for each question:
                - Use count_documents to display the number of documents contained in the result.
                - Display the first document in the results using pprint.
                - Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
            - Which establishments have a hygiene score equal to 20?
            - Which establishments in London have a RatingValue greater than or equal to 4?
            - What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
            - How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
                
## Installation and Configuration 
- Python, Pandas, PPrint, MongoDB  
	
- Files included with repository include the README, NoSQL_analysis, NoSQL_setup_starter, and Resources folder