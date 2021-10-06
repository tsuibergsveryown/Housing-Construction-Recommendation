Project 2 Presentation

### Data Science Problem Statement ###

## Overview ##
As the millennials (those who are born between 1981-1997) are taking the housing market by storm, 
they are looking for something different than previous generations of home buyers. 
Nearly 48% Canadians aged 25 to 35 currently own their home, and a quarter of these 
homeowners purchased a property during the coronavirus pandemic. As mortgage rate fell to 
historically low levels and the competition for entry-level housing lessened, young people
saw a window of opportunity and went for it. 

In addition, Covid-19 has shifted many millennials location from big cities to suburb for 
affordability housing as more companies are open for work-from-home arrangement. 

Our dataset from Ames, IA is a good dataset to study for because 
Ames is 3.5 hours drive away from a big city (Kansas City), and Ames is well known as the 
home of Iowa State University, with leading agriculture, design, engineering, and 
veterinary medicine colleges.


## Objective ##
As a real restate developer company, how do we position ourself better in comparison to our
competitors, to take advantage of this current trend / phenomenon? 
What parts of a house should we allocate our resource to when building new housing for 
the Millennials to maximize our profit? 

This project aims to identify the top 5 areas to prioritize when constructing our blueprint
& building the new houses to stand out from our competitors in order to maximize our sale
price for the real estate construction project. 


## Page 4 - 5 ##
Here we find some of the highest correlation between these features and the Sale Price.
There are total of 16 features that have high positive correlation with the Sale Price, 
ranging from features such as Total Room Above Ground, fireplace equality to the most obvious
features External Quality & Overall Quality of a house.
There are more than 60 features that have low positive/negative correlation with the 
Sale Price, and here are some of the examples. 
Hence, we are not going to use them in determining sale price of a home.

## Page 6 - 8 ##
So what really determine the final sale price of a home?

Our baseline here is that as long as the feature has more than 50% of correlation with
the Sale Price, then we are putting them into our machine learning model when we predict
the Sale Price later on. The rationale behind this is that these features are some of the
most important aspects that the homebuyers are considering when they purchase their home.
And that's why they drive up the sale price of these sold houses from our data. 

The total features we are considering to determine the sale price are sitting at 16 features
from the original dataset of 80 features. 
However, we have decided to drop 1 feature in our model - Garage Area
- because it is highly correlated to Garage Cars. Well, the rationale here is self-explanatory,
because when you are able to park more cars in your garage, you'd have bigger garage size.
However, having a large Garage Area does not neccessary mean that you'd have more
space to park cars, because some of the garage area could be built for storage cabins, 
which could take away some space to park 1 or 2 cars.

We are also adding 2 extra features that we created from 3 original features. They are Garage
Cars with Kitchen Quality, and Garage Cars with Living Area (above ground). 

You can see from the scatter plots here that both garage cars and living area above ground are
positively correlated with Sale Price. To be precise, they are only around 65% correlated for Garage
Cars, 68% for Kitchen quality, and 70% for Above Ground Living Area. However, when you 
combine the Garage Cars & Kitchen Quality as one single feature, the correlation with Sale
Price increase to 78%. And the same thing with Garage Cars & Living Area, the correlation 
with Sale Price is even better - 80%.

This could potentially mean that when a buyer is not so into the number of cars that they 
can park in their Garage, but combining with either bigger living area space or kitchen 
quality, they could potentially be more interesting in this house. This could be the home
buyers consist of a couple, where she doesn't care much about garage space, but she cares
more about the kitchen area (or the size of living area), and her partner doesn't care 
much about the kitchen area but cares more about the garage space to but his stuff and cars.
This could explain why these 2 new features we created have way higher correlation to Sale
Price when combined.


## Page 9 ##
Now we look at how our model performs. Our model performs fairly decent among the training
Data and the Testing Data. The two score are very close with each other, which means that 
our model is learning from the training that we told it to do. The bias and variance are
fairly balanced. 

This means that the 16 + 2 features that we chose earlier are working well in determining 
the Sale Price of a home. This brings to our conclusion that we should prioritize these 
features when we are constructing our next real estate project.

## Page 10 - 12 ##
So these are the top 5 features to pay attention to when building the new houses, because 
they have the highest correlation with the Sale Price. In addition, when we can, we should 
increase the size of living area above ground, as well as the garage area when we can.

What I'd NOT recommend to do is to keep the front/back yard size big, and the house small. 
This false combination will most likely not generate higher sale prices for your newly built 
houses. To remind everyone, our targeted demographic buyers are the majority millennials, 
not the minority millennials that are millionairs. 

We have to take special note that this dataset is missing the modern amenities data.
We also have to mention that the dataset we use are not suitable for cities Sale Price
prediction. It only serves a recommendation for suburban area houses that have similar 
features as the city of Ames, IA. In order to generalize to cities, we'd need to revise 
our model to add features such as modern amenities data of a city. 


--- END ---

Here I'm recommending the top 5 areas to put our priorities to when building our blueprints
and houses, so that we can maximize sale prices to generate higher profit: 
1. Kitchen Quality
2. Garage Finish
3. Full bathrooms above ground
4. Fireplace quality
5. Total rooms above ground

And when lot size permits, we should focus ourselves to maximize the sizes in:
1. Above ground living area (in square feet)
2. Garage area size