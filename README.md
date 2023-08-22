# Cyclistic

The provided SQL script involves various steps for data preparation, cleaning, and analysis of ride data from the Cyclistic company, comparing member and casual riders. Here's a summary of the work done in each section:

1. **Combining Data:**
   - Tables for each month's ride data are combined into a single table called `combined_data`.

2. **Data Cleaning:**
   - A table named `TripData` is created by selecting relevant columns from the `combined_data` table.
   - Unwanted columns are removed to clean the data.

3. **Calculating Ride Length:**
   - The ride lengths are calculated by finding the difference between the start and end times of each ride.
   - Negative ride lengths are corrected to zero for data integrity.

4. **Normalization:**
   - Several lookup tables are created for rideable types (`rideable_type`), stations (`station_data`), user categories (`user_cat_data`), and calendar dates (`calendar`).

5. **Joining Tables:**
   - The normalized lookup tables are joined with the main ride data (`master_table`) to create a comprehensive table called `joined_tables`.

6. **Exploratory Data Analysis (EDA):**
   - Various EDA queries are performed to gain insights into the data.
   - Ride length statistics, including averages and maximums, are calculated.
   - Ride distribution analysis by user category, day of the week, month, hour, etc., is performed.

7. **Aggregated Summary:**
   - An aggregated summary table is created, containing information about user categories, rideable types, dates, quarters, months, days of the month, days of the week, and hours.
   - The summary includes total ride lengths, average ride lengths, ride counts, and counts of short, average, and long rides.

The script mainly focuses on cleaning, transforming, and analyzing the Cyclistic ride data. It calculates statistics and creates summary tables to provide insights into the behavior of member and casual riders, ride lengths, and ride distribution patterns over different time periods.
