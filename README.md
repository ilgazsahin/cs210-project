# cs210-project

The primary motivation behind this project was to gain a deeper understanding of my personal habits and lifestyle. By analyzing various aspects of my daily life - including physical activity and social media usage - I aimed to uncover insights that could lead to healthier habits, more efficient time management, and overall wellbeing. The data for this project was sourced from multiple personal devices and applications. The step count data is extracted from my iphones's Apple Health App. Instagram Data is extracted from my Instagram account which included details about likes, saved posts, and messages, offering a glimpse into my social media interaction patterns.
Python scripts are used to parse JSON and XML files, converting raw data into structured formats like pandas DataFrames. This stage involved handling timestamps, extracting relevant fields, and formatting the data for analysis. 

# DATA ANALYSIS 
# Exploratory Data Analysis (EDA):
Step Count Analysis: Utilizing pandas and matplotlib, the step count data was visualized to observe daily, seasonal, and yearly trends. This included plotting the total steps per year, analyzing seasonal distributions, and calculating the average steps by day of the week. Since the step data encompassed a broader date range compared to the energy burned and sleep duration data, it was chosen for more in-depth analysis. Although the sleep duration and active energy data were limited, visualization techniques, such as those provided by matplotlib, were effectively used to analyze these datasets as well.

Instagram Data Analysis: This analysis involved examining likes, saved posts, and message data. Key activities included counting likes and saves per day, visualizing trends over time, and assessing the average like counts for each day of the week. By leveraging the daily counts of liked and saved posts, along with the total messages sent to my most interacted friends, I created a daily activity score ranging from 0 to 100. This innovative approach, utilizing existing data, helped me gain insights into my activity levels on Instagram.

Then to see the relation between daily step count data and daily activity score a graph was plotted. By visualizing these two sets of data on the same graph i have observed ,how my physical activity (as measured by step counts) correlates with my Instagram activity.

After visualization correlation coefficient and the p-value has been calculated and following are the findings: 
# Correlation coefficient: -0.08191364706806224
This value is between -1 and 1, where -1 indicates a perfect negative correlation, 0 indicates no correlation, and 1 indicates a perfect positive correlation.
A coefficient of -0.0819 suggests a very weak negative correlation between daily steps and Instagram activity scores. This means that as one variable slightly decreases, the other slightly increases, but the relationship is weak.

# p-value: 0.1218489060777037
A p-value less than 0.05 typically indicates that the correlation is statistically significant.
In this case, the p-value is greater than 0.05, which means there is not enough evidence to conclude that the correlation is statistically significant.

# Model Training and Testing:
Using linear regression i have used existing step count and instagram activity score data behaviour to predict future data based on historical trends .The data is split into training (80%) and testing (20%) sets without shuffling. This preserves the chronological order, which is important in time series analysis. Then, a linear regression model is trained on the training set. But it can be said that those models was not as efficient as expected due to limeted data. 
Then a trend analysis has been conducted.


# Findings: 
Every year, I aim to become more physically active. Observing the change in my total step count data over the years has been a motivating factor, as there has been a significant increase in yearly total step counts since 2019. Based on the Instagram activity scoring system that I've created, I gained insights into the content I consumed over the past year. Observing the negative correlation between my activity score and step count in some parts of the dataset made me realize that I can increase physical activity to reduce the time I spend on social media.

# Limitations and future work:
While conducting this project, I encountered several limitations. The limited data on sleep duration and active energy burned restricted my ability to analyze and correlate certain variables. In fact, my initial plan for this project differed in some aspects. I had intended to use my location data to analyze the walkability of the cities I had visited in the past year. However, I discovered that my location service was not enabled to collect my location data. Consequently, I enabled location data collection, and I plan to conduct different research next year using my step count and location data.



