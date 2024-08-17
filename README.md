
# NoSQL Challenge

## Overview
This project is focused on working with NoSQL databases, specifically MongoDB, to analyze data from the UK Food Standards Agency. The analysis was conducted to assist the editors of a food magazine, *Eat Safe, Love*, in evaluating food hygiene ratings across various establishments in the United Kingdom.

## Project Structure
The project is divided into three main parts:

### Part 1: Database and Jupyter Notebook Set Up
In this section, we set up our MongoDB database and Jupyter notebook environment.
1. Imported the data from the `establishments.json` file into a MongoDB database named `uk_food` with a collection named `establishments`.
2. Connected to the database and confirmed successful data import.
3. Displayed a document from the `establishments` collection using `find_one` and `pprint`.

### Part 2: Update the Database
This part involved modifying the database as per the magazine editors' requests.
1. Inserted a new restaurant, "Penang Flavours," into the `establishments` collection.
2. Updated the `BusinessTypeID` for "Penang Flavours" after querying for the correct ID.
3. Removed all establishments under the Dover Local Authority from the database.
4. Converted certain number values (like `latitude`, `longitude`, and `RatingValue`) from strings to their appropriate numeric data types.

### Part 3: Exploratory Analysis
Finally, an exploratory analysis was performed to answer specific questions posed by the magazine editors. The analysis included:
1. Identifying establishments with a hygiene score of 20.
2. Filtering establishments in London with a `RatingValue` of 4 or higher.
3. Finding the top 5 establishments with a `RatingValue` of 5, sorted by the lowest hygiene score, nearest to "Penang Flavours".
4. Counting establishments in each Local Authority area with a hygiene score of 0, and sorting these results by the highest count.

## Files Included
- `NoSQL_setup_starter.ipynb`: The Jupyter notebook for setting up the MongoDB database.
- `NoSQL_analysis_starter.ipynb`: The Jupyter notebook used for performing the exploratory analysis.
- `Resources/establishments.json`: The JSON file containing the data used in this project.
- `README.md`: This file, containing details about the project, setup instructions, and overview of the tasks performed.

## Instructions to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/maslla100/nosql-challenge
   ```
2. Install the necessary dependencies:
   ```bash
   pip install pymongo pandas
   ```
3. Start Jupyter Notebook and run the cells in `NoSQL_setup_starter.ipynb` to set up the database.
4. Run the cells in `NoSQL_analysis_starter.ipynb` to perform the exploratory analysis.


---

### Contact
For any questions or issues, please contact Luis.Llamas@maslla.com
```



