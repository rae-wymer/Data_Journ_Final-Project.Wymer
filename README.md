# Data_Journ_Final-Project.Wymer
J124 Final Project Repository documenting my analysis of Bicycle Collisions in San Francisco's Mission District from 2018-2023 
# <h1>Story Pitch 
In San Francisco, bike collisions have been a major saftey risk and problem. Each year, around 30 people die and many more are injured due to collisions and road saftey problems. For cyclists, key streets are often dangerous or hotspots for accidents and in recent years the city government has implemented changes to the street rules and bike-lane design in order protect residents. Most of this work has been through Vision Zero SF — a road saftey policy with planned actions and education efforts to decrease collisions. 

My data analysis focused on tracking collisions in San Francisco's Mission District where Visions Zero is piloting a new design for bike-lanes. This is one of the most dangerous neighborhoods to bike in and the data showed that Valencia Street, where the new proected bike lane is being piolted, is the most common road for a collision. My investigation will be tracking the saftey of this neighborhood since 2018 and where cyclists are at risk. I will analyze common locations for collisions, established a year-by-year comparison, understand the severty of these accidents and try to understand if these efforts by San Francisco's city government are effective. 

As my story continues, I plan to build of the foundation of information and understanding my data anaylsis will give me by speaking with impacted parties and looking into the funding for traffic saftey programs. These will expand the scope of my story and allow me to hold the city government accountable for the policies.   
#
<H2>Possible Sources </H2>
  
    1. Kimberly Leung: Valencia Bikeway Improvements Project Manager for SFMTA 
       - kimberly.leung@sfmta.com
       Kimberly Leung works on the Liveable streets team for SF Municipal Transit Association and has been running the Valencia Bikeway Improvements Project. Her perspective would be key in understand how the project is being organized and excuted. Additionally, she would provide answers to any accountablity issues that come up when assesing and interviewing for the effectiveness of this project.  
    2. Luke Borheimer: a local transportation advocate 
        - lukebornheimer@gmail.com
        Luke Borheimer has been openly against the Valencia Bikeway Improvements Project. He has been using his twitter to docuemnt issues and hazards along the street. He would be able to provide the prespective for cyclists using the new bike-lanes and share the public opinion on it.
<H2> Aditional Sources </H2>
City data:  

[Traffic Crashes](https://data.sfgov.org/Public-Safety/Traffic-Crashes-Resulting-in-Injuries/kn4t-hihx)

This is a city map of all Traffic Crashes in San Francisco which resulted injury. If I was to expand this investigation to a citywide project I would use this data to map and specify exactly where injuries occured and which neighborhoods to focus on. This would add both great context and additional scope to my story while grounding it.

SFMTA Funding: 

[Budget](https://www.sfmta.com/sites/default/files/reports-and-documents/2022/04/4-19-22_mtab_item_12b_consolidated_budget_-_book.pdf)

This document includes a breakdown of the entire SFMTA budget and shows exactly how much money is going into this Vizion Zero project. This would be a way to analyze and interrogate the effectiveness of these infrastructure projects and the work by SF Vision Zero. By comparing this with data on colisions I will add deeper level of analysis to see the impact that this money has had. 

# <h1>Data Used   
  
  I based by data analysis off San Francisco city data through the [TransBASE Dashboard](https://transbase.sfgov.org/dashboard/dashboard.php)
  
<h2> Analysis 1: How do bicycle collisions compare year by year? Which parties are usually at fault in these collisions?</h2>

Data Ananlysis and Visualization Process:
* Created a pivot table with columns selected for year and values as COUNTA for case_id which counted every single row of data. 
* To seperate data by year, I applied a filter to the year column of my dataset and created an indivdual datawrapper map for each year. The data inlcudes latitude and longitude cordinates for each collision so that allowed me to plot the data in Datawrapper through a symbol map. 
* To analyze the a single year's data I had datawrapper create a symbol and color palete based on the description logged for "party_1" which is the party at fault in each collision.
* I then repeated this for each year from 2018 to 2023. Once the data was plotted I added key markers for georaphical context of main street names and intersections in the neighborhood.

Screehshot of Pivot Table: number of cases per year

<img width="355" alt="Screen Shot 2023-08-10 at 2 27 57 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/d5e52e14-d70f-4f36-a79e-9d7e9892bced">

Screenshot of Pivot Table: Party_1/Party at Fault 

<img width="272" alt="Screen Shot 2023-08-10 at 2 31 35 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/51436883-0df7-413b-b341-89d5c282fd4c">


<h3> 2018 </h3> 

   ![bfJOZ-bike-collisions-in-sf-mission-neighborhood-2018 (2)](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/8b234972-aba6-421b-bcce-35bab6165e4c)

 [Link to data visualization](https://datawrapper.dwcdn.net/bfJOZ/4/)

<h3> 2019 </h3>

![oAn1F-bike-collisions-in-sf-mission-neighborhood-2019](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/1321841a-86e9-4cef-b7e1-af3efa01a66f)

 [Link to data visualization](https://datawrapper.dwcdn.net/oAn1F/1/)

<h3> 2020 </h3>

![eos7S-bike-collisions-in-sf-mission-neighborhood-2020](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/3092991b-5e57-4aa5-909b-cb0b326c5178)

 [Link to data visualization](https://datawrapper.dwcdn.net/eos7S/1/)

<h3> 2021 </h3>

![8nfLD-bike-collisions-in-sf-mission-neighborhood-2021](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/081d050f-a265-471b-992f-8b74cf6e3fa1)

 [Link to data visualization](https://datawrapper.dwcdn.net/8nfLD/1/)

<h3> 2022 </h3>

![4E5WH-bike-collisions-in-sf-mission-neighborhood-2022](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/8dbf717a-788d-4cc4-9050-9ddd74cc9cfd)

Link to data visualization [Google](https://www.google.com/)

<h3> 2023 </h3>

![6qb8u-bike-collisions-in-sf-mission-neighborhood-2023](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/41faf04b-81c9-469b-ad3f-cd2855322665)

Link to data visualization [Google](https://www.google.com/)

<h2> Analysis 2: How severe have these bicycle collisions been?</h2>

* I created a pivot table with a column seperating this data into the different logged collision severity [ Fatal, Injury (Complaint of Pain), Injury (Other Visible), Injury (Severe)]. I added rows to seperate the data by year to see how the collision severity changed over time and used COUNTA of case_id for individual values 

* Then I coppied this table into datawrapper to create a bar chart and visualize the analysis. I created a chart and found a grouped bar chart to be a suitable way to visualize this data. Once created I selected a color which would not seem correlated with death or injury ( I felt that would be a insensitive visualization). I decide to show increased intensity of the injury by using a darker shade of the color as the injury type became more severe.

Pivot Table 

<img width="681" alt="Screen Shot 2023-08-10 at 2 55 09 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/6da90584-7b8b-4755-bbac-bc8f1be57c04">

<h3> Collision by Year and Injury </h3>

![6ikz0-collisions-by-year-and-injury (2)](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/40478e31-da0c-485a-a291-4d4c2ec8440b)

Link to visualization [Google](https://www.google.com/)

<h2> Analysis 3: What are the major collision types? </h2>

* I created a pivot table which isolated the data of each major collision type and counted the amount of rows of data (or number of collisions) which fit each cateogry. 
* Then, I copied this data over into datawrapper to create a bar chart of this. Unlike other data visualizations so far I did not filter by year.

Pivot Table 

<img width="339" alt="Screen Shot 2023-08-10 at 3 03 04 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/a21158f8-a132-42a6-b0b4-4158f39cfc01">

<h3> Collision Types for 2018-2023 </h3>

![3GlV3-collision-types-for-2018-2023](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/642287d5-14f1-45c9-99b7-2b40c3fdc8d3)

Link to visualization  [Google](https://www.google.com/)

<h2> Analysis 3: Which streets are the most common sites for collisions? </h2>

* I created a pivot table with the data of the primary road for bicycle collision and filtered this data to have it sorted from most to least common primary roads.
* I copied this data into a chart on datawrapper to create a bart chart.

Pivot Table

<img width="204" alt="Screen Shot 2023-08-10 at 3 24 34 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/732ffa2d-48db-480b-8b98-7ff3f2951e67">

<h3> Most Common Primary Road for Collisions </h3>

![rpsLW-most-common-primary-road-for-collisions-](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/25cdaefa-47f8-4ea3-999f-e10f59383bb0)

Link to visualization  [Google](https://www.google.com/)

<h2> Analysis 4: How many bicycle collisions occured each year since 2018? </h2>

*  I created a pivot table of the number of collisions COUNTA case_id and sepeated them by year 2018-2023
*  I transfered this over into Datawrapper to create a column chart that had a horizontal axis for year and vertical axis for number of collisions.

  Pivot Table
<img width="297" alt="Screen Shot 2023-08-10 at 3 33 28 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/6a5dbddb-d5b7-49bc-ab13-176a39297195">

<h3> Number of collisions each year in the Mission </h3>  

![r3yub-number-of-collisions-each-year-in-the-mission](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/524505a6-4cbf-4e98-8b04-89d00043ca2a)

Link to visualization [Google](https://www.google.com/)

<h2> Analusis 5: Which parties are often at fault in these collisions? </h2>

*  I created a pivot table organizing the data of all collisions in my timeframe by the party_1/party at fault. I then sorted the data in decending order from most often at fault to least.
*  I copied this data over into Datawrapper and created a table of this data.

Pivot table

<img width="215" alt="Screen Shot 2023-08-10 at 3 49 58 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/e69ee195-a1c3-48e7-b590-5e8f5a28ef90">

<h2> Party at fault in bicycle collisions </h2>

![5PVNI-party-at-fault-in-bicycle-collisions (1)](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/be33b08b-3548-4794-a481-6f47791c30d8)

Link to visualization [Google](https://www.google.com/)

