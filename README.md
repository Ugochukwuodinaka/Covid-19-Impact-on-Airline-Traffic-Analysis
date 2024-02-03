# Covid-19-Impact-on-Airline-Traffic-Analysis-(2020)
![](Covid-19_Impact_on_Airport_Traffic_image.jpg)

## Table of Contents
- [Project Overview](#project-overview)
- [About The Dataset](#about-the-dataset)
- [Tools Used](#tools-used)
- [Visuals in Power BI:](#visuals-in-power-bi)
- [View and Interact With Power BI Dashboard Report](#view-and-interact-with-power-bi-dashboard-report)
- [Recommendations on How To Mitigate or Control the Impact of Pandemics on Airport Traffic](#recommendations-on How-to-mitigate-or-control-the-Impact-of-pandemics-on-airport-traffic)

## Project Overview
### Introduction:
The outbreak of the Covid-19 pandemic in 2020 led to unprecedented disruptions across various sectors, with the airline industry being one of the hardest-hit. This project aims to analyze the impact of the Covid-19 pandemic on global airline traffic patterns during the year 2020. By leveraging data analysis techniques, we seek to gain insights into how travel restrictions, lockdown measures, and public health concerns affected air travel behavior worldwide.

### Problem Statement:
The outbreak of the Covid-19 pandemic in 2020 has severely impacted the global airline industry, leading to unprecedented disruptions in air travel patterns. As countries implemented various containment measures, including travel restrictions and lockdowns, airline traffic experienced significant fluctuations, with profound implications for airlines, airports, and related stakeholders. However, there remains a critical need to systematically analyze the extent and nature of these disruptions, understand the underlying factors driving changes in airline traffic behavior, and identify actionable insights to inform future strategies and policies. This analysis project focuses on 4 countries which are: The Unuted States of America (USA), Canada, Australia and Chile.

This project seeks to address the following key questions:

- What is the total flight recorded for this analysis?
- What is the total traffic impact?
- What is the average percent of baseline?
- What is the total flights recorded by Country?
- What is the number of Airports, Countries and Cities in this analysis?
- What is the overall traffic impact by Country? Use a chart.
- With the help of a chart, display the flights trend monthly was recorded within the period of this analysis?
- Using a chart, show the contributions of different Airports to the overall traffic impact?
- Using geospatial mapping, showcase the percentage of baseline by Airport, Country, Stae and City?
- What actionable insights can be derived from the analysis to assist stakeholders in the aviation industry and policymakers in adapting strategies and mitigating future risks associated with similar crises?

### Expected Outcomes:

- Total Flight Recorded: The analysis will provide the total number of flights recorded within the specified period, offering a comprehensive view of the scale of air traffic during the time frame under consideration.

- Total Traffic Impact: By comparing pre-pandemic levels of air traffic with those during the pandemic period, the analysis will quantify the total impact on air traffic, providing insights into the severity of disruptions experienced by the airline industry.

- Average Percent of Baseline: Calculating the average percentage of baseline traffic will offer a standardized measure to gauge the overall reduction in air travel activity relative to pre-pandemic levels.

- Total Flights Recorded by Country: This outcome will present a breakdown of the total number of flights recorded for each country, enabling a comparative analysis of the impact across different regions.

- Number of Airports, Countries, and Cities: Providing counts of airports, countries, and cities included in the analysis will offer contextual information about the scope and geographic coverage of the dataset.

- Overall Traffic Impact by Country (Chart): A chart depicting the overall traffic impact by country will visually illustrate the varying degrees of disruption experienced across different countries.

- Monthly Flight Trend (Chart): Visualizing the monthly flight trend will enable stakeholders to identify temporal patterns and fluctuations in air travel activity over the course of the analysis period.

- Contributions of Different Airports (Chart): Displaying the contributions of different airports to the overall traffic impact will highlight the relative importance of various air transportation hubs in shaping the overall traffic patterns.

- Geospatial Mapping of Baseline Percentage: Using geospatial mapping, the analysis will showcase the percentage of baseline traffic by airport, country, state, and city, offering a spatial perspective on the distribution of air traffic disruptions.

- Actionable Insights: Drawing from the analysis results, actionable insights will be derived to assist stakeholders in the aviation industry and policymakers in adapting strategies and mitigating future risks associated with similar crises. These insights may include recommendations for route optimization, capacity planning, health and safety protocols, policy adjustments, and crisis management strategies.

### About The Dataset
This dataset shows traffic to and from the Airport as a Percentage of the Traffic volume during the baseline period. The baseline period used for computing this metric is from 1st Feb to 15th March 2020. The dataset gets updated monthly. This data is publicly available from [Geotab](https://www.geotab.com/). The dataset is in .csv file and can be viewed or downloaded [here](covid_impact_on_airport_traffic.csv)

The dataset is made up of 11 columns and 7,248 rows of data. Here is a breakdown of the column details:

- AggregationMethod: This column indicates the method used for aggregating or summarizing the data. Here, the data is aggregated on a daily basis.
  
- Date: This column represents the date for which the data is recorded. It typically follows a standardized date format (e.g., YYYY-MM-DD) and indicates the specific time point or period to which each data entry corresponds.

- Version: This column denotes the version or iteration of the dataset. It may indicate updates, revisions, or modifications made to the dataset over time, allowing users to track changes and ensure data integrity.

- AirportName: This column contains the name or identifier of the airport associated with each data entry. It identifies the specific airport location to which the data pertains, facilitating analysis and interpretation based on geographic context.

- PercentOfBaseline: This column provides a measure of the percentage deviation from a baseline value. In the context of airline traffic data, it represents the percentage of normal or pre-pandemic levels of air traffic for each observation, indicating the extent of disruption or recovery in air travel activity.

- Centroid: This column contain geographical coordinates (latitude and longitude) representing the central point or centroid of the airport location. It enables spatial analysis and visualization, allowing users to map and analyze data based on airport locations.

- City: This column specifies the city or urban area associated with each airport. It provides additional geographic information to complement the airport name, helping users identify the location of airports within specific cities or metropolitan areas.

- State: This column indicates the state or province (if applicable) where the airport is located. It further refines the geographical context of each airport, particularly in countries with administrative divisions such as the United States, Canada, or Australia.

- ISO_3166_2: This column contain the ISO 3166-2 code corresponding to the state or province where the airport is located. ISO 3166-2 is a standardized coding system used to represent country subdivisions, facilitating data interoperability and cross-referencing with other datasets.

- Country: This column specifies the country where the airport is situated. It provides the highest level of geographical context for each data entry, enabling analysis and comparison of data across different countries or regions.

- Geography: This column contain additional geographical information or descriptors related to each airport location. It could include details such as geographical regions, continents, or other spatial attributes that help classify and organize airport locations within a broader geographic framework.

### Tools Used
1. Power Query Editor
    - Was used to:
        1. Extract,
        2. Transform, and
        3. Load all the datasets for this analysis.
           
2. Power BI (Was used to create reports and dashboard for this analysis)
    - The following Power BI Features were incorporated:
        1. DAX,
        2. Quick Measures,
        3. Page Navigation,
        4. Filters,
        5. Tooltips

### ETL Process using the Power Query Editor:
1. Ttranslated all the colume headers in Swedish language to English for easy understanding
2. Duplicated the Centroid column into 2 more columns: "Centroid 1" and "Centroid 2"
3. Split the duplicated Centroid columns by delimeter.
4. Split the duplicated Centroid columns by position.
5. Changed the Centroid 1 and Centroid 2 datra types to 'text'.
6. Changed their column names to Longitude and Latitude.
7. Changed the Date column type to 'date'.
8. Made sure there is no null values or missing data.

**Raw Data**
![](Raw_Data.png)

**Final query editor screenshot**

![](Power_Query_Eitor_1.png)

## Visuals in Power BI:
![](Covid-19_Impact_On_Airport_Traffic_Analysis(2020)_Dashboard.jpg)

#### Analysis:
From the analysis, i made the findings below:
- The Total Flight Record is 7,247.
- The Average Percentage of Baselie is 66.65%.
- The total number of Airports is 28.
- The Total Traffic Impact is 483,000.
- Total Number of Airport Countries in this analysis is 4
- While the Total Number of Airport Cities is 27.
- Looking at the Total flights recorded by the 4 countries in this analysis, USA had the most number of flights which was 4,441, followed by Canada with 2,311 flights, Australia is next with 57 flights, and lastly, Chile with 238 flights. As we can see, there are variations in these numbers by countries. Let's run a more detailed analysis on them:
     1. Both the USA and Canada have larger populations and more extensive aviation industries compared to Australia and Chile. This inherently leads to higher levels of air travel 
        activity in these countries, irrespective of external factors.

     2. International Travel Hubs: Major cities in the USA and Canada, such as New York, Los Angeles, Toronto, and Vancouver, are significant international travel hubs. They attract a 
        large volume of passengers and facilitate numerous flight connections, contributing to higher overall flight numbers.

     3. Economic Activity and Business Travel: The USA and Canada are home to numerous multinational corporations and have strong economies. This results in substantial business travel 
        activity, which translates to higher demand for flights, particularly between major business centers and corporate hubs.

     4. Geopolitical Factors: The geographical proximity of the USA and Canada to other major global destinations, as well as their political and economic ties with various countries, 
        can influence the volume of international flights operating to and from these countries.

     5. However, it's important to note that the significant disparity in flight numbers between the USA and Canada compared to Australia and Chile during the early part of 2020 can 
        also be attributed to the onset of the Covid-19 pandemic. By January 2020, the Covid-19 outbreak had begun to spread globally, leading to widespread travel restrictions, border 
        closures, and a decline in passenger demand for air travel.

     6. As a result, the USA and Canada, being more connected to global travel networks and having larger aviation industries, likely experienced a higher volume of flights in the early 
        part of 2020 compared to Australia and Chile. However, as the severity of the pandemic increased and travel restrictions intensified, all countries would have seen significant 
        reductions in flight numbers compared to previous years.
     7. Generally, compared to the previous years, these 4 countries experienced lesser flight schedules, due flight restrictions that happened in 2020 due to the destructive impact of 
        the covid-19 pandemic not just in these 4 countries in this analysis, but globally.

- In the context of this analysis, the term "overall traffic impact" refers to the net change or deviation in air traffic activity compared to a baseline or reference period. The specific numbers associated with each country represent the magnitude of this impact, measured in some standardized unit (such as flight counts for this analysis) that allows for comparison across different regions or time periods.

     1. USA: With an overall traffic impact of 286,271, this indicates a substantial net change in air traffic activity within the United States during the specified period. The 
        positive value suggests an increase in air traffic relative to the baseline, while a negative value would imply a decrease.

     2. Canada: Similarly, Canada's overall traffic impact of 178,893 reflects the net change in air traffic activity within Canada during the analyzed period. Again, a positive value 
        indicates an increase in air traffic, while a negative value would signify a decrease.

     3. Australia: Australia's overall traffic impact of 9,702 indicates a comparatively smaller net change in air traffic activity within Australia during the specified period.

     4. Chile: Chile's overall traffic impact of 8,157 represents the net change in air traffic activity within Chile during the analyzed period.

     5. These values provide quantitative insights into how the Covid-19 pandemic, or other factors under consideration, affected air traffic patterns in each country. A higher overall 
        traffic impact suggests a more significant deviation from normal or baseline levels of air traffic, while a lower impact indicates a relatively smaller deviation.

- In the Flight Trend by Month linechart, it is evident that there are fluctuations in air travel activity throughout the year, with certain months experiencing higher or lower percentages relative to a baseline reference point. Below is an analysis of these trends:

     1. Initial Impact of Covid-19 Pandemic (March to May): The percentage of baseline in March is 445, indicating a significant decline in air travel activity compared to pre-pandemic 
        levels. This decline likely corresponds to the initial onset of the Covid-19 pandemic, as countries implemented widespread travel restrictions and lockdown measures to contain 
        the spread of the virus. In April and May, although still significantly below baseline levels, there is a gradual increase in the percentage of baseline (825 and 855, 
        respectively), suggesting a partial recovery or stabilization in air travel activity as some restrictions were lifted and travel began to resume cautiously.

     2. Summer Recovery (June to August): From June to August, there is a further increase in the percentage of baseline, indicating a continued recovery in air travel activity during 
        the summer months. The percentages range from 831 to 862, reflecting a gradual return to normalcy as travel restrictions eased, and consumer confidence in air travel began to 
        improve.

     3. Plateau and Fluctuations (September to November): In September and October, the percentage of baseline remains relatively stable, hovering around 835 to 868, suggesting a 
        plateau in air travel activity. However, there may be fluctuations within this period due to factors such as changing travel regulations, economic conditions, and regional 
        outbreaks of Covid-19. By November, there is a slight decrease in the percentage of baseline to 835, indicating a potential stabilization or modest decline in air travel 
        activity compared to the previous months.

     4. Year-End Decline (December): The percentage of baseline drops significantly in December to 56, indicating a sharp decline in air travel activity compared to the rest of the 
        year. This decline may be attributed to various factors, including holiday travel disruptions, increased Covid-19 cases and restrictions, and seasonal trends in air travel 
        demand.

     5. Overall, the analysis of flight trends by month highlights the dynamic nature of air travel activity throughout the year, with fluctuations influenced by external factors such 
        as the Covid-19 pandemic, government policies, economic conditions, and seasonal variations. 

- Here's an analysis of the contribution of different Airports to the Overall Traffic Impact of the Covid-19 pandemic:

     1. Decline in Air Travel Activity: The data reflects a significant decrease in air travel activity across various airports, as indicated by the lower percentages of baseline. This 
        decline can be attributed to the widespread implementation of travel restrictions, border closures, and lockdown measures in response to the Covid-19 pandemic.
    
     2. Regional Variation in Impact: While airports in Canada and the USA are among the top contributors to the overall traffic impact, they also experienced substantial reductions in 
        activity. Canadian airports such as Winnipeg International, Hamilton International, and Calgary International, despite ranking high in contribution, still witnessed notable 
        declines compared to pre-pandemic levels. Similarly, major US airports like Newark Liberty International, Daniel K Inouye International, and Chicago O'Hare International, while 
        significant contributors, also saw decreases in air traffic activity.

     3. Resilience of Some Airports: Despite the overall decline, certain airports displayed relatively higher levels of activity compared to others. For instance, Vancouver 
        International in Canada and Dallas/Fort Worth International in the USA maintained higher percentages of baseline, indicating a degree of resilience or adaptability to the 
        challenges posed by the pandemic.

     4. Impact on International Travel Hubs: International travel hubs such as Los Angeles International, Miami International, and John F. Kennedy International in the USA experienced 
        significant declines in activity. These airports typically handle a large volume of international flights, but the pandemic's disruption to global travel severely impacted their 
        operations.

     5. Global Connectivity Affected: Airports beyond North America, such as Kingsford Smith in Australia and Santiago International Airport in Chile, also witnessed declines in air 
        travel activity. This indicates the global nature of the pandemic's impact on air travel and underscores the interconnectedness of aviation networks worldwide.

     6. Economic and Operational Challenges: The data reflects the economic and operational challenges faced by airports during the pandemic, including reduced passenger demand, 
        cancellations of flights, and financial strains on airport operations. These challenges have necessitated adaptive measures and strategic planning to navigate the uncertainties 
        of the aviation industry in 2020 and beyond.

     7. Overall, the analysis of airport contributions to the overall traffic impact underscores the profound effects of the Covid-19 pandemic on air travel activity worldwide.

- The geospatial map showing the percentage of baseline by airports, longitude, latitude, countries, states, and cities offers a detailed visualization of the impact of the Covid-19 pandemic on air travel activity in 2020. Here's an analysis based on the provided information:

     1. Spatial Distribution of Impact: The map provides insights into the spatial distribution of the percentage of baseline across different airports, countries, states, and cities. 
        Areas with higher percentages may indicate regions that were less severely affected by the pandemic's disruptions, while lower percentages signify areas with more significant 
        declines in air travel activity.

     2. Identification of Hotspots and Coldspots: By overlaying the data on a geospatial map, it becomes possible to identify hotspots and coldspots of air travel activity represented 
        by the sizes of the blue bubbles. Bigger bubbles correspond to regions with relatively higher percentages of baseline, indicating resilience or adaptability to the challenges 
        posed by the pandemic. smaller bubbles, on the other hand, represent areas with lower percentages, signifying more significant disruptions.

     3. Impact on Transportation Hubs: The map highlights the impact of the pandemic on transportation hubs, such as airports, which serve as critical nodes in global air travel 
        networks. Airports with lower percentages of baseline may include major international hubs that experienced substantial declines in passenger traffic, flight operations, and 
        cargo shipments due to travel restrictions and reduced demand.

     4. Regional Disparities and Economic Implications: Regional disparities in the percentage of baseline reflect variations in the severity of the pandemic's impact on air travel 
        activity. These disparities can have economic implications, affecting industries dependent on tourism, business travel, and international trade. Regions heavily reliant on air 
        transportation may experience economic downturns due to reduced connectivity and mobility.

     5. Policy Response and Recovery Strategies: The geospatial map can inform policymakers, aviation industry stakeholders, and public health officials in assessing the effectiveness 
        of policy responses and designing recovery strategies. Understanding the spatial patterns of air travel activity can help prioritize resource allocation, target interventions, 
        and support the gradual resumption of air travel in the post-pandemic period.

## View and Interact With Power BI Dashboard Report
You can view and interact with this report [here](https://app.powerbi.com/view?r=eyJrIjoiNzUzZDA3YzEtNjI3Ni00NDRlLWFjMTEtNGUzNWUyYWY5Y2NmIiwidCI6IjdlYzI5NjU5LTNjZjItNGYzZi1hYmIzLWE3MjJlZGY3ZmYyZCJ9).The dashboard report on Covid-19 Impact on Airports Traffic (2020) analysis showcases an interactive visual of the project in power BI.

## Recommendations on How To Mitigate or Control the Impact of Pandemics on Airport Traffic

In conclusion, mitigating and controlling the impact of pandemics on airport traffic requires a multifaceted approach that involves proactive measures, effective coordination, and adaptive strategies. Here's a summary of key considerations:

- Preventive Measures: Implementing stringent health and safety protocols at airports, including temperature screenings, mandatory mask-wearing, enhanced cleaning and disinfection procedures, and social distancing measures, can help mitigate the spread of infectious diseases among passengers and airport personnel.

- Travel Restrictions and Screening: Implementing travel restrictions and screening measures, such as quarantine requirements, testing protocols, and travel advisories, can help limit the spread of pandemics by reducing the movement of infected individuals across borders and identifying potential cases early.

- Enhanced Communication and Coordination: Establishing robust communication channels and coordination mechanisms among airport authorities, government agencies, airlines, and public health authorities is essential for sharing information, coordinating response efforts, and implementing effective measures to contain outbreaks and mitigate their impact on airport traffic.

- Flexible Operations and Contingency Planning: Developing flexible operational plans and contingency measures that can be activated in response to changing epidemiological conditions, travel advisories, and government regulations is critical for maintaining airport operations, minimizing disruptions, and ensuring the continuity of essential services during pandemics.

- Investment in Technology and Infrastructure: Investing in technology and infrastructure upgrades, such as contactless check-in and boarding processes, automated screening systems, and enhanced ventilation systems, can help enhance the resilience of airports to pandemics by reducing person-to-person contact and minimizing the risk of transmission.

- Collaborative Research and Innovation: Promoting collaborative research and innovation in areas such as vaccine development, antiviral treatments, and epidemiological modeling can help advance scientific understanding of pandemics and inform evidence-based decision-making in mitigating their impact on airport traffic.

- Community Engagement and Public Awareness: Engaging with local communities, passengers, and stakeholders through public awareness campaigns, educational initiatives, and community outreach efforts can help build trust, promote compliance with health guidelines, and foster a culture of resilience and solidarity in responding to pandemics.








