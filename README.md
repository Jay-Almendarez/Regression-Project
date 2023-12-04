# Regression-Project
---
## Project goals
- Viably predict the property value of a home off key drivers found in the zillow dataset
- Present deliverables to zillow data science team in the form of a presentation
---
## Project description
One of the most variable investments that a lot of people find themselves involved in is owning a house. At first glance it seems like there's almost no rhyme or reason why two very similar looking houses could vary in price so wildly. That's what we're hoping to solve here (at least in a specified area of California that is). We believe we can find key causes in property value and reliably predict the approximate price of a home based on categories like how many bathroooms it has, or how large it is altogether.

---
## Project planning (lay out your process through the data science pipeline)
- Planning: Indicate plan of action and begin laying out framework for project
- Acquisition: Acquire data from Zillow with listed specifications of 'Single Family Properties'
- Preparation: Clean data (removing any null values, coding columns to numeric columns, scaling and ultimately splitting data)
- Explore: Determine key drivers and begin asking questions of the Zillow data
- Model: Determine optimal model for predicting property value and attempt to beat baseline
- Delivery: Present findings through a presentation to data science peers
---
## Initial hypotheses and/or questions you have of the data, ideas
There is likely a noticable difference in value when comparing counties, I'd like to explore this more and see if it's significant. Initial predictions are as follows: Square footage of a home and the amount of bathrooms are the most significant to the overall value of the home.

---
## Data dictionary
| Feature | Definition | 
| :- | :- |
| Beds | Number of bedrooms a house has. |
| Baths | Number of bathrooms a house has. (1.5 = one and a half bathrooms) |
| <font color='red'>Square Feet</font> | Area of flooring in a house |
| Value | Property value of a house |
| Year Built | Year of house being completed |
| County | County the house is located in 0 = LA, 1 = Orange, 2 = Ventura |

---
## Methods to Reproduce
- The data pulled from MySQLWorkbench is in the form of a .csv included in this repository, so the simplest process for replication would be to download the file immediately.
- There is also a wrangle.py file that will determine if the .csv exists and bring it in if it does, and if it does not, it will use a env file with MySQLWorkbench login info (username, password, and url) to obtain and cache the data
---
## Key findings, recommendations, and takeaways from your project.
- Separating data by County resulted in change in optimal modeling
- Square footage had high correlation to home value
- Recommend creating models for each county to improve predictive strength of models
---
