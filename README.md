# Zuber Database Analysis
## Introduction
A SQL project to analyze taxi ride data for Zuber, a ride-sharing company, to test a hypothesis about the impact of weather on ride frequency.    
### Company Overview
Zuber is a burgeoning ride-sharing company set to revolutionize transportation in Chicago. Committed to providing efficient and convenient rides, Zuber aims to optimize the passenger experience through data-driven insights and innovative solutions.   
### Project Overview
As an analyst at Zuber, I addressed critical business challenges by conducting an in-depth analysis of taxi ride data, utilizing SQL JOIN to correlate trips and weather records. This resulted in valuable insights into passenger behavior and external factors' impact on rides, empowering Zuber's strategic decision-making.    

## Description of the data 
A database with info on taxi rides in Chicago:  

**neighborhoods table**: data on city neighborhoods  
- name: name of the neighborhood  
- neighborhood_id: neighborhood code  

**cabs table**: data on taxis   
- cab_id: vehicle code  
- vehicle_id: the vehicle's technical ID  
- company_name: the company that owns the vehicle  

**trips table**: data on rides  
- trip_id: ride code  
- cab_id: code of the vehicle operating the ride  
- start_ts: date and time of the beginning of the ride (time rounded to the hour)  
- end_ts: date and time of the end of the ride (time rounded to the hour)  
- duration_seconds: ride duration in seconds  
- distance_miles: ride distance in miles  
- pickup_location_id: pickup neighborhood code  
- dropoff_location_id: dropoff neighborhood code   

**weather_records table**: data on weather  
- record_id: weather record code  
- ts: record date and time (time rounded to the hour)  
- temperature: temperature when the record was taken  
- description: brief description of weather conditions, e.g. "light rain" or "scattered clouds"

## Table scheme
![Image (17)](https://github.com/chiangsuanne/Zuber-Database-Analysis/assets/108243961/e731db81-278b-4a10-a286-d49e9a127f7f)

## Project Analysis
**Analyzing Taxi Ride Patterns**    
Explored and analyzed taxi ride data, identifying key patterns and preferences. This enhanced our understanding of passenger behavior and the impact of external factors on rides. The analysis involved using SQL JOIN to link trips and weather records in Zuber's database.    

**Investigating Taxi Ride Statistics for November 15-16, 2017**    
Determined the number of taxi rides for each company during this period, providing insights into ride frequency. The results were presented by sorting the data based on trips_amount.    

**Analyzing Taxi Rides for "Yellow" or "Blue" Companies from November 1-7, 2017**    
Calculated the number of rides for companies containing the keywords "Yellow" or "Blue," highlighting ride volume. The data was grouped by company_name to show relevant statistics.    

**Assessing Ride Frequency for Selected Taxi Companies in November 2017**    
Investigated ride counts for specific companies (Flash Cab and Taxi Affiliation Services) and provided a comparative analysis with other companies grouped as "Other." This enhanced our understanding of market dynamics and competition.    

**Analyzing Loop to O'Hare Airport Rides on Rainy Saturdays**    
Examined ride duration changes based on weather conditions, identifying patterns in rides from the Loop to O'Hare on rainy Saturdays. Utilized neighborhood data, weather records, and SQL queries to categorize conditions, extract relevant trip data, and obtain ride durations.    

## Project Insight
### Conclusion
1. The five enterprises with the most considerable number of trips are (descending order): Flash Cab, Taxi Affiliation Services, Medallion Leasing, Yellow Cab, and Taxi Affiliation Service Yellow
2. There is a discrepancy in the average trip duration from the Loop to O’Hare International Airport on rainy Saturdays, as it is longer on bad weather conditions, which suggest that weather conditions may play a notable role in influencing ride durations.  
### Suggestions for Further Improvement or Business Outcomes 
1. **Enhance Service Allocation:**  
    - Allocate resources strategically by recognizing the popularity of Flash Cab, Taxi Affiliation Services, Medallion Leasing, Yellow Cab, and Taxi Affiliation Service Yellow. Consider optimizing fleet distribution based on demand patterns for these key players.  
2. **Weather-Responsive Pricing Models:**  
    - Implement dynamic pricing models that consider weather conditions, offering incentives during inclement weather to encourage more ridership. This could involve discounts during rainy Saturdays to attract passengers during adverse conditions.  
3. **Route Optimization:**  
    - Optimize routes or provide alternative routes during bad weather conditions, especially for routes like the Loop to O'Hare International Airport, where longer trip durations are observed. This can improve overall customer satisfaction and potentially reduce operational costs.  
4. **User-Friendly Weather Notifications:**  
    - Implement a feature within the app to notify users about potential weather-related impacts on ride durations, allowing for informed decisions and better user experience.
5. **Continuous Data Analysis and Adaptation:**
    - Establish a continuous analysis process to monitor changing trends in customer preferences and external factors. This ongoing assessment will enable the company to adapt quickly to evolving market dynamics and stay ahead of competitors.
6. **Customer Feedback Mechanism:**
    - Implement a feedback mechanism to gather customer opinions specifically related to weather conditions, allowing the company to fine-tune services based on real-time user experiences and expectations during different weather scenarios.
7. **Collaborations with Top-Performing Companies:**  
    - Explore partnerships or collaborations with the top-performing taxi companies to strengthen the company's market position and potentially offer joint promotions or services to a broader customer base.  
