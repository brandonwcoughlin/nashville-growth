# nashville-growth
# Growth in Nashville

Capstone Project for Data Analytics Cohort 12 at Nashville Software School

Nashville has been growing rapidly since I moved here in 2017. In this project I dive deeper into what that growth has looked like over the years. What neighborhoods is this growth happening in? What types of buildings are being built, and where?

## Motivation

Seven years ago, I graduated from college in my home state of Ohio. Shortly after, I made the move from Ohio—a state known for its flat landscapes, cornfields, and Skyline Chili—to the vibrant city of Nashville, Tennessee. Upon settling into East Nashville, I quickly grew fond of the neighborhood’s energy and rapid growth. The area, like much of the city, was booming with new home constructions, commercial developments, and an ever-expanding list of restaurants. It seemed that every corner had something new, adding to my appreciation of living in Nashville.

During my time as a Sales Engineer at a commercial ventilation company, I had the opportunity to manage and design projects for various types of buildings, including hotels, apartments, schools, government facilities, and restaurants. This role gave me an inside view of the ongoing development across the city. However, I noticed that this growth was not evenly distributed. My curiosity about the emergence of "hot spot" neighborhoods led me to dive deeper into the data. By leveraging publicly available datasets, I transformed my curiosity into data-driven insights to better understand the patterns of urban development in Nashville.

## Data Question

What types of buildings are being built in Nashville?

What can we expect to see for Nashville's growth moving forward?


## Data Challenges

### Irrelevant Zip Codes

<img width="573" alt="Screenshot 2024-10-19 at 10 29 10 AM" src="https://github.com/user-attachments/assets/83b0200f-aa8e-4999-b415-46be0117c3f3">

Since the data is self-reported by contractors through permit applications, there were inconsistencies, particularly with the zip codes. Some of the zip codes provided did not correspond to any valid zip codes within the city and, as a result, had to be removed from the dataset to ensure accuracy. 

### Time Traveling Contractors

<img width="571" alt="Screenshot 2024-10-19 at 10 32 36 AM" src="https://github.com/user-attachments/assets/d404f3e4-551f-4c5e-9e4f-66eec1129877">

Given that the data is self-reported by contractors, there were some discrepancies in the dates between when permits were applied for and when they were issued. In several cases, permits appeared to be issued before the application date. As I don't believe Nashville employs time-traveling contractors, I attributed these anomalies to human error in the submission process. Consequently, some of the dates were considered irrelevant and excluded from the analysis.

## Data Sources and Tools Used

### Data Sources

This project utilizes data published by data.nashville.gov, sourced from two Metro Nashville departments. The data is updated nightly at 2:00 a.m. Additionally, the Neighborhood Association Boundaries map is incorporated to provide geographical context.

* Building Department Permit Applications: Includes data from the application process through to issuance, rejection, or withdrawal. However, it does not contain information on estimated construction costs.

* Building Department Permits Issued: Provides a rolling three-year history of issued permits.

### Tools

* Python
* Jupyter Notebook
* PowerBI
* MS Excel

## Approach

* ETL Process: I extracted data from data.nashville.gov to assess the structure and determine the necessary transformations for further analysis. The datasets were then loaded into Python for in-depth analysis and manipulation.
* MVP Determination: I identified the minimum viable product (MVP) by selecting the most effective charts, graphs, and visuals for the analysis. This process also included planning the design and functionality of an interactive dashboard in Power BI.
