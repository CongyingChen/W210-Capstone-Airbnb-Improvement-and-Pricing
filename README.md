# W210-Capstone-Airbnb-Improvement-and-Pricing

## Improve Your Airbnb Listing for Higher Price and Better Revenue

### Problem
Individual hosts of Airbnbs are interested in improve the quality of their listings by asking suggestions from experts. 

In traditional hotel industry, hotel consulting company can sit down with hotel owners for a couple of weeks and exam every aspect of their operation and room quality, then have a detailed written report or tools to improve the quality of the hotel. 

However, vacation rental industry doesn’t not necessary need this detailed consulting service, which was used for a hotel with hundreds of room. It only need some website or app that can take one copy of the URL of their listing and tell them where they can improve compared to the most popular listings and get their price increased. 

### Related Work of Interest
Airbnb itself or some other third party companies provide quality improvement service to hosts, but it is qualitative, time consuming and expensive. 

Currently according to my research, there is no company or websites analysing quality of a listing and give suggestion to the host based on public Airbnb and neighbourhood data. 

### Further Issues to Tackle 
Connection to Airbnb API
Input from hosts about their budget of renovation or improvement projects, preference, or another personalized data that is not available public. 
Output as a quality report and paragraphs of suggestions of the listing, instead of just check mark or scores of some variables.

### Target Users
Airbnb Hosts
Airbnb service or quality improvement specialist 

### Data
http://insideairbnb.com/get-the-data.html
Listings.csv.gz
	Number of rooms
	Summary
	Space 
	Description
	Neighbourhood overview
	Cancellation policy
	Reviews per month
	
Reviews.csv.gz
	date 
reviewer_id 
reviewer_name 
Comments

Neighbourhoods.geojson
Compare listing in the same neighbourhood.

Calendar.csv.gz
	Date
Price
	Min & Max night
Availability

Other Data can be 
Traveler segmentation - representing different expectation and purchase power for a room.
Graph of that listing - whether it is a attracting graph, or whether it matches the expectation from time 
	
	
### Possible Data Science Techniques/Technical Requirements
NLP for review analysis
Time Series Analysis to forecast occupancy
Machine Learning to predict how popular one listing is, and the weight/importance of each features, then make suggestions of improving the quality. 
Data visualization about quality score with multiple variables and timespane.
	

### References
 InsiderAirbnb: http://insideairbnb.com/get-the-data.html
 AirDNA:https://www.airdna.co/vacation-rental-data
 






