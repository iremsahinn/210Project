**Analysis of Personal Netflix Streaming Data**

**Introduction**

The purpose of this project was to explore my personal streaming data on Netflix, focusing on the correlation between the genre of what I watched, time of day, and device type I used for streaming. My hypothesis was: "During afternoon hours, I am more likely to watch romantic content on larger screens like TVs, while evenings see a higher viewership of comedies on PC devices." The purpose of this study is to get understanding about my own watching habits and preferences.

**Data Source**

For my main data, I requested my streaming history data from Netflix, and got 4 years of streaming data. But, to test my hypotheses, I need genres and types of what I watched. I provide these values and add them into my Data. 

**Data Preprocessing**

The Netflix streaming data was initially loaded into a Pandas DataFrame for manipulation and analysis. Main preprocessing steps included:

1. Separating 'Start Time' into distinct date and time columns.
1. Simplifying 'Title' by removing season and episode number
1. Formatting "Duration" in terms of a minute.
1. Categorizing 'Device Type' into broader classes (Mobile, Tablet, PC, TV).
1. Dropping rows where 'Latest Bookmark' was 'Not latest view' since they are duplicates.
1. Creating a 'Part of Day' feature to categorize viewing times into morning, afternoon, evening, and night.

**Exploratory Data Analysis (EDA)**

To investigate the data, several visualizations were made, including:

- The distribution of genres demonstrated the variety and frequency of genres watched.
- The distribution of device types revealed preferences for various streaming devices.
- Time of day analysis revealed viewing patterns across different times.
- Additional analyses included genre popularity trends over time, and a correlation heatmap to understand relationships between different variables.

**In-Depth Analysis**

I tested my hypothesis using statistical methods and visualizations:

- Chi-Square tests were applied to inspect the association between time of day and genre, and between time of day and device type.
- An analysis of the interaction effect shed light on how genre, device type, and time of day all affect watching habits.

**Findings**

The analysis revealed several key insights:

- Top 3 watched genres were:
  - Teen TV Shows             149 times
  - TV Dramas                 137 times
  - Romantic TV Dramas        129 times
    
![image](/Picture1.png)
- Top 3 watched types were:
  - Emotional      204 times
  - Heartfelt      161 times
  - Suspenseful    156 times
    
![image](/Picture2.png)

- Mostly, TV was preferred to watch movies and TV series.
  
![image](/Picture3.png)
- Looking at the viewing time, more viewing was done in the afternoons.
  
![image](/Picture4.png)
- The interaction effect analysis vividly illustrated these patterns, showing a clear preference for romantic genres on TVs in the afternoon and comedies on PCs in the evening.

- There was a significant association between the time of day and the genre of content watched. Romantic content was more frequently watched during afternoon hours, aligning with the hypothesis.
  
![image](/Picture5.png)

- The choice of device also varied with the time of day. Larger screens like TVs were preferred during the afternoon.
  
![image](/Picture6.png)

- Consumption of comedy content increases in evenings, predominantly on PC devices, supporting the hypothesis.
  
![image](/Picture7.png)

- Consumption of romantic content increases in afternoons, predominantly on TV devices, supporting the hypothesis.
  
![image](/Picture8.png)

- Watching duration and watched device has the highest correlation compared to other categories.
  
![image](/Picture9.png)

- Device type usage/popularity is not change considerably over the time. It tends to maintain similar popularity rates.
  
![image](/Picture10.png)


**Conclusion**

The idea was validated by the data analysis, which showed clear trends in streaming behavior depending on the device type, content genre, and time of day. These results offer insightful information about individual viewing preferences and can guide future selections of devices and content for the best possible streaming experience.
