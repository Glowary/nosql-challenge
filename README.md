# NoSQL Challenge

## Part 1: Database Set Up

### 1. Import Data
1.  Open Terminal and import the dataset with `mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`
3. Check the database by:
	-   List the databases in MongoDB and confirm that `uk_food` is listed.
	-   List the collections in the `uk_food` database to ensure that `establishments` is present.
	-   Find and display one document in the `establishments` collection using `find_one` and display with `pprint`.
	-   Assign the `establishments` collection as a variable for furture use.

### 2. Modification
1.  Add the new halal restaurant in Greenwich to the database with the code provided. 
2. Find the `BusinessTypeID` for "Restaurant/Cafe/Canteen" and return only the `BusinessTypeID` and `BusinessType` fields.
3. Update the new restaurant with the `BusinessTypeID` found. 
4. Check how many documents contain Dover. Remove any establishments within the Dover from the database, and confirm the number of documents after deletion.
5. Update number values:
    -   Use `update_many` to convert latitude and longitude to decimal numbers.
    -   Use `update_many` to convert `RatingValue` to integer numbers.
