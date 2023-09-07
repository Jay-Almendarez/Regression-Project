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
| Feature | Definition | \n",
    | :- | :- |\n",
    | Senior Citizen | If a customer is a senior citizen, 0 = No, 1 = Yes |\n",
    | Tenure | The amount of months a customer has been with or is currently with company |\n",
    | <font color='red'>Monthly Charges</font> | Amount a customer is charged monthly |\n",
    | Total Charges | Cumulative amount a customer has paid |\n",
    | Gender | If a customer is male or female, 0 = Female, 1 = Male |\n",
    | Has Partner | If a customer has a partner, 0 = No, 1 = Yes |\n",
    | Has Dependents | If a customer has dependents, 0 = No, 1 = Yes |\n",
    | Has Multiple Lines | If a customer has multiple lines, 0 = No, 1 = Yes |\n",
    | <font color='red'>Contract</font> | Type of contract customer has, 0 = Month-to-month, 1 = One year, 2 = Two year|\n,
    | Internet Service | Type of Internet Service customer has, 0 = No internet service, 1 = DSL, 2 = Fiber optic |\n,
    | Has Automatic Payment | If a customer has automatic payment, 0 = No, 1 = Yes |\n",
    | Has Amenities | If a customer has a majority of amenities from (tech_support, online_security, paperless_billing, streaming_movies, online_backup, streaming_tv, device_protection), 0 = No, 1 = Yes |\n,
    | <font color='red'>Has Internet Service</font> | If a customer has internet service, 0 = No, 1 = Yes |\n",
    | Churn (Target) | If a customer has churned, False = No, True = Yes |
---
## Instructions or an explanation of how someone else can reproduce your project and findings (What would someone need to be able to recreate your project on their own?)
- The data pulled from MySQLWorkbench is in the form of a .csv included in this repository, so the simplest process for replication would be to download the file immediately.
- There is also a wrangle.py file that will determine if the .csv exists and bring it in if it does, and if it does not, it will use a env file with MySQLWorkbench login info (username, password, and url) to obtain and cache the data
---
## Key findings, recommendations, and takeaways from your project.
- WIP
---