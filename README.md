# PWD-DTI-Batam-DatSci-Module-2-Capstone-Project

# ✨✨✨ Capstone_Project_2_Purwadhika ✨✨✨

# TransJakarta Data Analysis


## Presentation (visual overview)
TransJakarta Tableau Story Link: https://public.tableau.com/app/profile/rizqi.ahmad.kurniawan/viz/Module2DTI-DSCapstoneProjectTransJakartaDB/TransJakartaStoryTableau?publish=yes   


## Quick Overview
- Capstone project for learning module 2 of Purwadhika DTI Data Science Program. 
- The project is a Data Analysis take on TransJakarta's April 2023 passenger transaction data in Tab. 

## General Overview
## 1. Background:
Transjakarta is the first Bus Rapid Transit (BRT) transportation system in Southeast Asia operating since 2004 in Jakarta, Indonesia. TransJakarta was designed as a mass transportation mode to support Indonesia’s Capital city’s around the clock activities. 
With the longest track in the world (251.2 km), as well as having 260 bus stops spread across 13 corridors. Transjakarta initially operates from 05.00 - 22.00 WIB, now it operates 24 hours available on certain corridors only. With its extensive network of routes and ease of use, Transjakarta has become the leading and favorite transportation for so called “Jakartans”. 
However, there are several problems that still lingers around and thus must be handled. Problems such as sexual harassment that still often occurs to women, pickpocketing, bus crashes, schedule punctuality, accumulation of passengers at bus stops, overcrowding inside the bus itself. All stemming from overcrowding and less than optimal fleet distribution and fleet schedule.

## 2. Problem Statement
Overcrowding has led to several of Transjakarta’s pre-existing problems aforementioned in the Background. Thus, Transjakarta wants to research on its “overcrowding” problem associated with fleet distribution and schedule to help evaluate and improve its services to passengers (“Jakartans”) 

## 3. Data
This data is the passenger data for the month of April 2023. It initially consists of 37,900 rows (reduced to 35,476 post-preprocessing) and 22 columns. The Data Can be seen as follows:

## 4. Data Analysis
Overcrowding can be identified through several variables that helps us measure overall quantity of passengers. These variables can also help describe the demography of our passengers in the form of customer segmentation. For this research, we are focusing on the variables that can be associated with “overcrowding”. These variables will be highlighted with the arrow (->) notation below:

### -> Biodata:
1.     transID: Unique transaction id for every transaction
2.     payCardID: Customers main identifier. The card customers use as a ticket for entrance and exit.
3.     payCardBank: Customers card bank issuer name -> Payment Gateway Analysis
4.     payCardName: Customers name that is embedded in the card.
5.     payCardSex: Customers sex that is embedded in the card -> Gender Analysis
6.     payCardBirthDate: Customers birth year -> Customer Segmentation by Age range
#### -> Journey (Trip Details):
7.     corridorID: Corridor ID / Route ID as key for route grouping. -> Corridor Analysis
8.     corridorName: Corridor Name / Route Name contains Start and Finish for each route. -> Corridor Analysis
9.     direction: 0 for Go, 1 for Back. Direction of the route. -> In/Out Analysis
#### -> Journey (Tap-In details): -
10.  tapInStops: Tap In (entrance) Stops ID for identifying stops name
11.  tapInStopsName: Tap In (entrance) Stops Name where customers tap in. -> Bus Stops Analysis (origin)
12.  tapInStopsLat: Latitude of Tap In Stops -> Geo Analysis
13.  tapInStopsLon: Longitude of Tap In Stops
14.  stopStartSeq: Sequence of the stops, 1st stop, 2nd stops etc. Related to direction. -> stopCount Analysis
15.  tapInTime: Time of tap in. Date and time -> Time-based Analysis
#### -> Journey (Tap-Out details):
16.  tapOutStops: Tap Out (Exit) Stops ID for identifying stops name
17.  tapOutStopsName: Tap out (exit) Stops Name where customers tap out. -> Bus Stops Analysis (destination)
18.  tapOutStopsLat: Latitude of Tap Out Stops > Geo Analysis
19.  tapOutStopsLon: Longitude of Tap Out Stops
20.  stopEndSeq: Sequence of the stops, 1st stop, 2nd stops etc. Related to direction. -> stopCount Analysis
21.  tapOutTime: Time of tap out. Date and time -> Time-based Analysis
#### -> Journey (Trip Details):
22.  payAmount: The number of what customers pay. Some are free. Some not. -> Revenue Analysis


## 5. Final Initial Hypothetical Thoughts (guiding concerns)
Overcrowding can be best described as a phenomenon where the quantity of people exceed the threshold of collective and overall comfort of a cohort of people. To mitigate such problems. We can list the overall data analysis research findings, along with recommendations such as addressing customer segments that majorly contributes to “overcrowding”, fleet distribution and schedule that accommodate peak demand hours based on some of its busiest corridors (and its stops) whilst accommodating concerns such as female passenger safety by way of dedicated female rows on buses and female-only buses. Such implementation requires a certain degree of supervision, hence the optimal number of staff and their respective distribution along with comprehensive CCTV coverage. 

“Overcrowding” stems from congestion, and congestion does not always happen at the bus but rather the bus stops itself. This might cause certain problems such as pickpocketing and uncomfortable waiting conditions. To reduce such congestion, Transjakarta can increase its number of fleets, along with the aforementioned fleet distribution and schedule. This will also lessen the already high operating hours that might result in unexpected vehicle breakdowns, which might further worsen the problem as a delay in supply might trickle down to the whole system’s operational efficiency


## Dependencies
- Python 3.x
- Tableau app
- Jupyter Notebook extension

