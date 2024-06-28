IPL 2024 Exploratory Data Analysis (EDA) Project

1. Introduction
   
   - Analyzed two datasets: `matches.csv` and `deliveries.csv` to derive meaningful insights about the IPL 2024 season.


2. Data Importing

   - Imported the datasets and displayed the first few rows to understand the structure and content.

3. Initial Data Exploration
   
   - Examined the shape, summary statistics, and data types of both datasets.

   - Checked for missing values and duplicates.

4. Data Cleaning
   
   - Matches Dataset (`matches.csv`):
     
     - Dropped unnecessary columns (`method` and `city`).

     - Removed rows with missing values in the `winner` column.

     - Filled missing values in the `player_of_match` column with 'Unknown'.

     - Replaced missing values in the `result_margin` column with the median value.
       
   - Deliveries Dataset (`deliveries.csv`):
     
     - Filled missing values in `extras_type`, `player_dismissed`, `dismissal_kind`, and `fielder` columns with 'None'.

5. Feature Engineering
   
   - Extracted year, month, and day from the date column.

   - Renamed `id` to `match_id` for clarity.

6. Merging Datasets
   
   - Merged `matches.csv` and `deliveries.csv` on `match_id` to create a comprehensive dataset.

7. Analysis and Visualization
   
   - Winning Percentage by Team:
     
     - Calculated the number of matches each team played and won.

     - Computed and visualized the winning percentage of each team.

   - Top 10 Batsmen by Total Runs:
    
     - Identified and visualized the top 10 batsmen based on total runs scored.

   - Top 10 Bowlers by Total Wickets:

     - Identified and visualized the top 10 bowlers based on total wickets taken.

   - Players with Centuries:

      - Filtered and listed players who scored 100 or more runs in a match.

