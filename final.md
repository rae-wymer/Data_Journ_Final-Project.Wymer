# Data_Journ_Final-Project.Wymer
J124 Final Project Repository documenting my analysis of Bicycle Collisions in San Francisco's Mission District from 2018-2023 
# <h1>Story Pitch 
In San Francisco, bike collisions have been a major saftey risk and problem. Each year, around 30 people die and many more are injured due to issues with road saftey. Key streets for cyclists are often dangerous or hotspots for accidents. In recent years the city government has implemented changes to the street rules and bike-lane design in order protect residents. Most of this work has been through Vision Zero SF — a road saftey policy with planned actions and education efforts to decrease collisions. The work of Vision Zero has been funded by San Francisco's city government.  

My data analysis focused on tracking collisions in San Francisco's Mission District where Visions Zero is piloting a new design for bike-lanes. The Mission is one of the most dangerous neighborhoods to bike in and the data showed that Valencia Street, where the new protected bike-lane is being piloted, is the most common site for collisions. My investigation will be tracking the saftey of this neighborhood since 2018. I will analyze common collision locations, establish a year-by-year comparison of collision data, understand the severty of these accidents and try to understand if the Vision Zero efforts by San Francisco's city government are effectivly making streets safer. 

As my story continues, I plan to build on the foundation of information and understanding my data anaylsis will provide by speaking with impacted parties and looking into the funding for traffic saftey programs. This will expand the scope of my story and allow me to hold the city government accountable for the policies.  I will use the data I have found on bike collisions and collision fatalities over the last 6 years to analyze and interrogate the effectiveness of these infrastructure projects and the work by SF Vision Zero. 

#<H2>Possible Sources </H2>

* Kimberly Leung: Valencia Bikeway Improvements Project Manager for SFMTA 
   - kimberly.leung@sfmta.com
     Kimberly Leung works on the Liveable Streets team for SF Municipal Transit Association and has been running the Valencia Bikeway Improvements Project. Her perspective would be key in understanding how the project is being organized and excuted. Additionally, she would provide answers to any accountablity issues that come up when assessing the effectiveness of this project.  
* Luke Borheimer: a local transportation advocate 
  - lukebornheimer@gmail.com
    Luke Borheimer has been openly against the Valencia Bikeway Improvements Project. A self descirbed transportation advocate, he has been using twitter to document and broadcast issues with the project. His prespective would showcase civilian opposition to the new project and he could potentially share any insights into the risks that cyclists face in San Francisco.
    
<H2> Aditional Sources </H2>
City data:  

[Traffic Crashes](https://data.sfgov.org/Public-Safety/Traffic-Crashes-Resulting-in-Injuries/kn4t-hihx)

This is a city map of all Traffic Crashes in San Francisco which resulted injury. If I was to expand this investigation into a citywide project I would use this data to map and specify exactly where injuries occured and which neighborhoods to focus on. This would add both great context and additional scope to my story while grounding it in the human experience. I could find areas where I would want to follow-up with in-person reporting and speak with people living or working in these neighborhoods to gain a sense of how these saftey issues materialize in their lives.

SFMTA Funding: 

[Budget](https://www.sfmta.com/sites/default/files/reports-and-documents/2022/04/4-19-22_mtab_item_12b_consolidated_budget_-_book.pdf)

This document includes a breakdown of the entire SFMTA budget and shows exactly how much money is going into this Vizion Zero project. This would be a way to analyze and interrogate the effectiveness of these infrastructure projects and the work by SF Vision Zero. By comparing this with data on colisions I will add deeper level of analysis to see the impact that this money has had. This could open up a new line of inquiry based around these funding structures and where local funds are being directed.  

# <h1>Data Used   
  
  I based by data analysis off San Francisco city data through the [TransBASE Dashboard](https://transbase.sfgov.org/dashboard/dashboard.php)

  I edited and cleaned my data in this google sheet [here](https://docs.google.com/spreadsheets/d/1c-rnJEkCzaIL5axiYhGUhjITkPGYHJ_htd6-VfwlHWE/edit#gid=2053104748) . To clean my data I expanded the orignal date format into 3 new columns for Year, Month, Day using =LEFT(F2,4) to isolate the year, =MID(F2,5,2) to isolate the month and =RIGHT(F2,2) to isolate the day. Then I combined this into a single column using =DATE(G2,H2,I2) before formating into MM/DD/YYYY using Format>Number>Date>03/14/2012. I left-aligned jumbled cells. I also reformated the time from Ex: 1902 into 7:02 PM using =(TEXT(TIME(VALUE(LEFT(K2,2)),VALUE(RIGHT(K2,2)), 0),"h:mm AM/PM")). 
 
<h2> Analysis 1: How do bicycle collisions compare year by year? Which parties are usually at fault in these collisions?</h2>

Data Ananlysis and Visualization Process:
* I created a pivot table with columns selected for year and values (COUNTA for case_id) to count every single row of data. 
* To seperate data by year, I applied a filter to the year column of my dataset.
* I created an indivdual Datawrapper map for each year. The data inlcudes latitude and longitude cordinates for each collision so that allowed me to plot the data in Datawrapper through a symbol map. 
* To analyze the a single year's data I had Datawrapper create a symbol and color palete based on the description logged for "party_1" which is the party at fault in each collision.
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

 [Link to data visualization](https://datawrapper.dwcdn.net/4E5WH/1/)

<h3> 2023 </h3>

![6qb8u-bike-collisions-in-sf-mission-neighborhood-2023](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/41faf04b-81c9-469b-ad3f-cd2855322665)

 [Link to data visualization](https://datawrapper.dwcdn.net/6qb8u/1/)

<h2> Analysis 2: How severe have these bicycle collisions been?</h2>

* I created a pivot table with a column seperating this data into the different logged collision severity [ Fatal, Injury (Complaint of Pain), Injury (Other Visible), Injury (Severe)]. I added rows to seperate the data by year to see how the collision severity changed over time and used COUNTA of case_id for individual values. 

* Then I copied this table into Datawrapper to create a bar chart and visualize the analysis. I created a chart and found a grouped bar chart to be a suitable way to visualize this data. Once created, I selected a color which would not seem correlated with death or injury ( I thought that would be a insensitive visualization). I decide to show increased intensity of the injury by using a darker shade of the color as the injury type became more severe.

Pivot Table 

<img width="681" alt="Screen Shot 2023-08-10 at 2 55 09 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/6da90584-7b8b-4755-bbac-bc8f1be57c04">

<h3> Collision by Year and Injury </h3>

![6ikz0-collisions-by-year-and-injury (2)](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/40478e31-da0c-485a-a291-4d4c2ec8440b)

 [Link to visualization](https://datawrapper.dwcdn.net/6ikz0/2/)

<h2> Analysis 3: What are the major collision types? </h2>

* I created a pivot table which isolated the data of each major collision type and counted the amount of rows of data (or number of collisions) which fit each cateogry. 
* Then, I copied this data over into Datawrapper to create a bar chart of this. Unlike other data visualizations so far I did not filter by year.

Pivot Table 

<img width="339" alt="Screen Shot 2023-08-10 at 3 03 04 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/a21158f8-a132-42a6-b0b4-4158f39cfc01">

<h3> Collision Types for 2018-2023 </h3>

![3GlV3-collision-types-for-2018-2023](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/642287d5-14f1-45c9-99b7-2b40c3fdc8d3)

  [Link to visualization](https://datawrapper.dwcdn.net/3GlV3/2/)

<h2> Analysis 3: Which streets are the most common sites for collisions? </h2>

* I created a pivot table with the data of the primary road for bicycle collision and filtered this to have it sorted from most to least common primary roads.
* I copied this data into a chart on Datawrapper to create a bart chart.

Pivot Table

<img width="204" alt="Screen Shot 2023-08-10 at 3 24 34 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/732ffa2d-48db-480b-8b98-7ff3f2951e67">

<h3> Most Common Primary Road for Collisions </h3>

![rpsLW-most-common-primary-road-for-collisions-](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/25cdaefa-47f8-4ea3-999f-e10f59383bb0)

  [Link to visualization](https://datawrapper.dwcdn.net/rpsLW/1/)

<h2> Analysis 4: How many bicycle collisions occured each year since 2018? </h2>

*  I created a pivot table of the number of collisions ( COUNTA case_id ) and seperated them by year for 2018-2023. 
*  I transfered this over into Datawrapper to create a column chart that had a horizontal axis for year and vertical axis for number of collisions.

  Pivot Table
<img width="297" alt="Screen Shot 2023-08-10 at 3 33 28 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/6a5dbddb-d5b7-49bc-ab13-176a39297195">

<h3> Number of collisions each year in the Mission </h3>  

![r3yub-number-of-collisions-each-year-in-the-mission](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/524505a6-4cbf-4e98-8b04-89d00043ca2a)

 [Link to visualization](https://datawrapper.dwcdn.net/r3yub/2/)

<h2> Analusis 5: Which parties are often at fault in these collisions? </h2>

*  I created a pivot table organizing the data of all collisions in my timeframe by the party_1/party at fault. I then sorted the data in decending order from most often at fault to least.
*  I copied this data over into Datawrapper and created a table of this data.

Pivot table

<img width="215" alt="Screen Shot 2023-08-10 at 3 49 58 AM" src="https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/e69ee195-a1c3-48e7-b590-5e8f5a28ef90">

<h2> Party at fault in bicycle collisions </h2>

![5PVNI-party-at-fault-in-bicycle-collisions (1)](https://github.com/rae-wymer/Data_Journ_Final-Project.Wymer/assets/140004445/be33b08b-3548-4794-a481-6f47791c30d8)

 [Link to visualization](https://datawrapper.dwcdn.net/5PVNI/2/)

