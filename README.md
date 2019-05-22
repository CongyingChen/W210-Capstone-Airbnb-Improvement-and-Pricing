## W210 Capstone Ideas

# Improve Your Airbnb Listing for Higher Price and Better Revenue

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
 



# Rory's Idea: First-time listing optimization on Airbnb


### Problem
Airbnb provides a platform for property owners to list their spare room or property online and rent to travelers. As a property owner who does not have too much experience with renting their room / apartment for a short term, figuring out what would be a fair daily rate to charge at the start can be challenging. While he / she can certainly use prices for other nearby listings as a reference, or look at the average price per footage in the area, these reference points may not serve as a very good anchor because each property is unique and other property owners may have different goals in mind when they set up pricing. Also, since he / she is making a new listing, there is no historical booking data to look back to, to understand price elasticity. The other special aspect of property rental pricing is seasonality - the property owner needs to find not just 1 optimal price, but rather optimal prices, for different periods of time. If your spare room is in or near coachella, you can expect much higher prices during the music festival days.

In addition to the challenge of setting the right price, emphasizing the right characteristics may also help make the listing more successful. If the property owner understands what drives renter’s willingness-to-pay, he/she can also tailor the descriptions in the listing / title accordingly.

### Target User / Customer
People interested in putting their room / apartment / house on Airbnb and become a host
 
### Data
Insideairbnb (http://insideairbnb.com/get-the-data.html) - listing, calendar, and reviews data for Airbnb in many cities at various times (this data does not ah ever occupancy rate - of course, but we could potentially use number of reviews as a proxy for how often a property is booked)

Large scale conjoint (ACBC) survey - to complement existing data and reveal underlying preferences of travelers when selecting accommodation. We will split our sample into different groups that go through trade off exercises for different types of destinations and travel purposes (business vs. leisure), since preferences will likely change accordingly

Weather, events, holiday data to infer seasonality


### Possible data science techniques:
Clustering (to identify similar listings)

Regression models (linear, decision tree, etc.) to predict occupancy rate at various price points

Conjoint utility modeling based on results from conjoint survey

Data Visualization

### Related research/products
Beyondpricing (https://beyondpricing.com/) is a dynamic pricing tool developed for property owners on Airbnb. However this tool focuses on optimizing and adjusting prices of existing listings based on forecasted booking curve (generated on historical data). I aim to focus on the “first time pricing” challenger instead of the “revenue management” challenge




