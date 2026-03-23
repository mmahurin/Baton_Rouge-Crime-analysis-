# Baton_Rouge-Crime-analysis-

In-depth analysis of Baton Rouge Police Crime Incidents data, addressing several key questions about crime patterns.

Data Loading and Initial Exploration: The notebook first loads the crime incident data into a pandas DataFrame and performs some basic data cleaning, such as converting date columns.

Highest Crime Committed Each Month (Question 1) & Overall (Question 3): The analysis consistently identifies THEFT as the most frequently occurring crime overall (17,420 incidents) and also as the highest crime committed in every single month of the dataset. This is supported by monthly counts and visualized with a bar chart showing theft trends over months and a pie chart illustrating theft's proportion relative to other crimes.

Neighborhoods with Highest Crime Rates (Question 2): The code groups crimes by neighborhood and finds that NORTH BATON ROUGE has the highest crime count (10,630 incidents), followed by Scotlandville (7,989) and Jones Creek (7,731). A horizontal bar chart visualizes the top 10 high-crime neighborhoods.

Day vs. Night Crime Rates (Question 4): The analysis divides crimes into 'Day' (6 AM to 6 PM) and 'Night' (6 PM to 6 AM). Statistical tests (Shapiro-Wilk for normality, followed by Mann-Whitney U test due to non-normality) reveal no significant difference in crime rates between daytime and nighttime, challenging common assumptions. Q-Q plots and a box plot further illustrate these findings.

Association Between Neighborhood and Crime Type (Question 5): The notebook categorizes neighborhoods and crime types by their frequency and performs a Chi-Square Test of Independence. The results indicate no significant association between the type of neighborhood (high vs. low crime frequency) and the type of crime committed (common vs. rare crimes). A clustered bar chart visualizes these distributions.

Linear Relationship Between Month and Crime Counts (Question 6): By aggregating total crime counts per month, the analysis calculates a Pearson correlation coefficient. It discovers a significant negative linear relationship (r = -0.7678, p = 0.0035), indicating a clear downward trend in crime counts over the year. A scatter plot with a linear trend line visually represents this decline.
