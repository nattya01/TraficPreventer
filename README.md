### TraficPreventer

# Our team 
1. 
TraficPreventer
2.
Omer Perach 
	0506780397 
	omerperach@gmail.com
Or Hapaz 
	0546387666 
	orharpaz1@gmail.com
Nattyi Akav 
	0532825665 
	nattya01@gmail.com
Anya Katz 
	0525715476 
	anyakatz63@gmail.com
3.
- Omer:
	M.Sc in genetics,
	Basic python and R capabilities
- Or:
	B.a in politics and geography
	Has experience as a front-end developer writing javascript with react, node.js in the server side and mongoDB  and SQL as databases
	Also very proficient in Excel and power BI
- Nattyi:
	Bs.c in statistics and economy
	3 years experience in risk and data analysis, writing automation rules, variables creation and qa. 
	Highly proficient in SQL, excel, tableau, R and SAS
	Basic knowledge in python
- Anya: 
	Bs.c in computer science with specialization of Computer vision
	Working with AI algorithms.
	4 years experience with Python.

# The data
4.
Link to Dataset: https://www.kaggle.com/usdot/nhtsa-traffic-fatalities
5.
Created by the National Highway Traffic Safety Administration (NHTSA) for the Kaggle.com data science projects.
6.
© 2018 Kaggle Inc

# Business questions 
7-9.
	Business questions 
	1)	Places or district in the US likely to be susceptible to more crashes – insurance company interest.
	2)	The police and the medical units weak places – zones where they don't respond fast.
	3)	 The roads authority in the US – which signs on the way and in which places are more crash "inviting"?
	4)	Analyzing intersect crashes alone and to suggest a model on how to build safer intersect or where is the dangers places around the intersect?
	Who (hypothetically) needs to review your business questions before you analyze?
	I think that the best person to review our business question is our target client; maybe what we think as a good business question is not question at all.
	Find an academic article(s) (patent or blog) that relates to data similar to yours:
	https://www.kaggle.com/ahmedlahlou/preventing-traffic-accidents-in-paris-with-ai
	https://medium.com/geoai/using-machine-learning-to-predict-car-accident-risk-4d92c91a7d57


# The variables (columns) 
10.


Variable Name	Description	Type	Possible values
State_number	Holds a numeric value for the state with federal district and inhabited territories 	Numeric	1-56 1-Alabama
56 - Wyoming
State_name	This data element identifies the state in which the crash occurred.	Categorial	Alabama, Alaska….
Consecutive_number	This data element is the unique case number assigned to each crash	Numeric	560086
number_of_vehicle_forms_submitted_all	Number of vehicles that were involved in the accident	Numeric	1,2,3….58
Number_of_motor_vehicles_in_transport_mvit	The number of vehicles that were involved which aren’t legally parked   	Numeric	1,2,3….58
number_of_parked_working_vehicles	This data element is a count of the number of parked and working vehicles involved in the crash	Numeric	1…11
number_of_forms_submitted_for_persons_not_in_motor_vehicles	This data element is the number of Person Forms (Not a Motor Vehicle Occupant) involved in the accident	Numeric	0,….,16
number_of_persons_not_in_motor_vehicles_in_transport_mvit	This data element is a count of the number of non-motorists in the crash. A non-motorist is defined as a pedestrian, a cyclist, an occupant of a motor vehicle not in transport.	Numeric	0,…,16
number_of_persons_in_motor_vehicles_in_transport_mvit	This data element is a count of the number of motorists in the crash. A motorist is a driver, passenger or unknown occupant type of a motor vehicle in-transport. 0-999 Number of Persons in Motor Vehicles In-Transport	Numeric	0,…,93
number_of_forms_submitted_for_persons_in_motor_vehicles	This data element is a count of the number of Person Level (Motor Vehicle Occupant) Forms that are applicable to this case (i.e., occupants).	Numeric	0,…,93
County	This data element records the location of the unstabilized event with regard to the County. The codes are from the General Services Administration’s (GSA) publication of worldwide Geographic Location Codes (GLC). 000 Not Applicable 001-996 Use GSA Geographical Codes 997 Other 998 Not Reported 999 Unknown	Numeric	1,…,999
City	his data element records the location of the unstabilized event with regard to the City. The codes are from the General Services Administration’s (GSA) publication of worldwide Geographic Location Codes (GLC). 0000 Not Applicable 0001-9996 GSA Geographical Codes 9997 Other 9898 Not Reported 9999 Unknown	Numeric	0,…,10000
Day_of_crash	This data element records the day of the month on which the crash occurred. 01-31 Day of the Month of the Crash -- Unknown	Numeric	1,…,31
Month_of_crash	This data element records the month in which the crash occurred.	Numeric	1,…,12

year_of_crash	This data element records the year in which the crash occurred. xxxx Year of the Crash	Numeric	2000,….,2016
Day_of_week	Holds the day of the week in which the accident occurred. 	Numeric	1,…,7
Hour_of_crash	This data element records the hour at which the crash occurred. 00-23 Hour -- Not Applicable or Not Notified 99 Unknown	Numeric	0,…24,99
Minute_of_crash	This data element records the minutes after the hour at which the crash occurred. 00-59 Minute -- Not Applicable or Not Notified 99 Unknown	Numeric	0,…,60,99
national_highway_system	If the crash occurred in a highway system. 	Numeric	0,1,9
Land_use	Numeic for land use – 1 (Rural), 2 (Urban), 6 (Trafficway Not in State Inventory), 8 (Not Reported) and 9 (Unknown).	Numeric	1,2,6,8,9
Land_use_name	1 (Rural), 2 (Urban), 6 (Trafficway Not in State Inventory), 8 (Not Reported) and 9 (Unknown).	Categorial	Rural, Urban, Trafficway not in state, Not reported, unknown
Functional_system	01 (Interstate), 02 (Principal Arterial – Other Freeways and Expressways), 03 (Principal Arterial – Other), 04 (Minor Arterial), 05 (Major Collector), 06 (Minor Collector), 07 (Local), 96 (Trafficway Not in State Inventory), 98 (Not Reported), and 99 (Unknown).	Numeric	1,…,7,96,98,99
Functional_system_name	01 (Interstate), 02 (Principal Arterial – Other Freeways and Expressways), 03 (Principal Arterial – Other), 04 (Minor Arterial), 05 (Major Collector), 06 (Minor Collector), 07 (Local), 96 (Trafficway Not in State Inventory), 98 (Not Reported), and 99 (Unknown).	Categorial	Interstate
Route_signing	This data element identifies the route signing of the trafficway on which the crash occurred. 1 Interstate 2 U.S. Highway 3 State Highway 4 County Road 5 Local Street – Township 6 Local Street – Municipality 7 Local Street – Frontage Road (Since 1994) 8 Other 9 Unknown	Numeric	1,…,9
Route_signing_name	This data element identifies the route signing of the trafficway on which the crash occurred.	Categorial	State Highway, Insterdate…
trafficway_identifier	This data element records the trafficway on which the crash occurred.	Text	Actual Posted Number, Assigned Number, or Common Name (30 characters) 999999999999999999999999999999 Unknown
trafficway_identifier_2	This data element records the trafficway on which the crash occurred.	Text	Actual Posted Number, Assigned Number, or Common Name (30 characters) 999999999999999999999999999999 Unknown
latitude	This element identifies the location of the crash using Global Position coordinates. This is the position of latitude	Numeric	36.81472222
longitude	This element identifies the location of the crash using Global Position coordinates. This is the position of longitude	Numeric	-76.34784167
special_jurisdiction	This data element identifies if the location on the trafficway where the crash occurred qualifies as a Special Jurisdiction even though it may be patrolled by state, county or local police	Numeric	0,…,9
special_jurisdiction_name	This data element identifies if the location on the trafficway where the crash occurred qualifies as a Special Jurisdiction even though it may be patrolled by state, county or local police	Categorial	No Special Jurisdiction 
First_harmful_event	This data element describes the first injury or damage producing event of the crash. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	0,…,9
First_harmful_event_name	This data element describes the first injury or damage producing event of the crash.	Categorial	Rollover/Overturn
manner_of_collision	This data element describes the orientation of two motor vehicles in-transport when they are involved in the “First Harmful Event” of a collision crash. If the “First Harmful Event” is not a collision between two motor vehicles in-transport it is classified as such. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	0,…,9
manner_of_collision_name	This data element describes the orientation of two motor vehicles in-transport when they are involved in the “First Harmful Event” of a collision crash. If the “First Harmful Event” is not a collision between two motor vehicles in-transport it is classified as such.	Text	Not Collision with Motor Vehicle in Transport (Not Necessarily in Transport for 2005-2009)	
relation_to_junction_within_interchange_area	This data element identifies the crash's location with respect to presence in an interchange area. The coding of this data element is done in two sub-fields (see also C20B) and is based on the location of the “First Harmful Event” of the crash. 0 No 1 Yes 8 Not Reported 9 Unknown	Numeric	0,…,1
relation_to_junction_specific_location	This data element identifies the crash's location with respect to presence in or proximity to components typically in junction or interchange areas. The coding of this data element is done in two sub-fields (see also C20A) and is based on the location of the “First Harmful Event” of the crash. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	1,…,20,99
relation_to_junction_specific_location_name	This data element identifies the crash's location with respect to presence in or proximity to components typically in junction or interchange areas. The coding of this data element is done in two sub-fields (see also C20A) and is based on the location of the “First Harmful Event” of the crash.	Categorial	Non-Junction
Type_of_intersection	This data element identifies and allows separation of various intersection types. 1 Not an Intersection 2 Four-Way Intersection 3 T-Intersection 4 Y-Intersection 5 Traffic Circle 6 Roundabout 7 Five-Point, or More 10 L-Intersection 98 Not Reported 99 Unknown	Categorial	Not an Intersection	
work_zone	This data element identifies a motor vehicle traffic crash in which the first harmful event occurs within the boundaries of a work zone or on an approach to or exit from a work zone, resulting from an activity, behavior, or control related to the movement of the traffic units through the work zone. 0 None 1 Construction 2 Maintenance -- Construction or Maintenance 3 Utility 4 Work Zone, Type Unknown -- Not Reported	Categorial	None, Construction…
relation_to_trafficway	This data element identifies the location of the crash as it relates to its position within or outside the trafficway based on the “First Harmful Event.” For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	1,…,99
relation_to_trafficway_name	This data element identifies the location of the crash as it relates to its position within or outside the trafficway based on the “First Harmful Event.”	Categorial	“On Rodway”
Light_condition	This data element records the type/level of light that existed at the time of the crash as indicated in the case material. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	1,…,9
Light_condition_name	This data element records the type/level of light that existed at the time of the crash as indicated in the case material.	Categorial	Daylight, Dark – Lighted,…
atmospheric_conditions_1	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	1,…,10,99
atmospheric_conditions_1_name	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material.	Categorial	snow,clear,…
atmospheric_conditions_2	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315
Numeric	1,…,12
atmospheric_conditions_2_name	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material.	Categorial	Cloudy, No Additional Atmospheric Conditions	
atmospheric_conditions	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Numeric	1,..,10,99
atmospheric_conditions_name	This data element records the prevailing atmospheric conditions that existed at the time of the crash as indicated in the case material. For more info on the codes, please look at section in the pdf: https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812315	Categorial	Clear, Cloudy,…
School_bus_related	This data element identifies if a school bus, or motor vehicle functioning as a school bus, is related to the crash. 0 No 1 Yes -- Not Reported	Boolean	True, False
rail_grade_crossing_identifier	This data element identifies if the crash occurred in or near a rail grade crossing. 0000000 Not Applicable xxxxxxA Six Digits Followed by One Alphabetic Valid F.R.A. Code 9999999 Unknown	Text	00000000
number_of_fatalities	This data element records the number of fatally injured persons in the crash. 01-99 Number of Fatalities that Occurred in the Crash.	Numeric	0,…,99
Number_of_drunk_drivers	This data element records the number of drunk drivers involved in the crash. 00-99 Number of Drunk Drivers Involved in the Fatal Crash.	Numeric	0,..,3
timestamp_of_crash	This data element records the date and time on which the crash occurred.	Date and Time	08/01/2015 07:11:00
