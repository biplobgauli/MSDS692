# POLICE SHOOTING IN THE US : FACT VS MYTH

# Introduction
For the MSDS Practicum 1, I wanted to dive deeper into the issue that has been in the news quite frequently and been a concerning topic: police shooting. There was also in incident earlier this year where a military officer was harassed by a policeman. This was a first time I had heard of such incident. In this case, the military officer was a person of a color, which led me to this project and dive deeper into whether people of color are impacted the most by police shooting.

# Agenda
- Problem description
- Datasets
- Data prepping
- Exploratory data analysis
- Visualizations
- Correlation
- Forecasting
- Conclusion

# Problem description
Here are the questions I want to answer in this project:
- Are people of color being impacted the most?
- Are there any other socio-economic factors Tied to shooting?
- How does the shooting trend will look like in the future?



Datasets
- Primary shooting dataset (Washington Post)
  - Shooting dataset
  - Contains descriptive information for Shooting from 2015- 2021
  - Close to 6k records
  - Name
  - Age
  - Gender
  - Race
  - Location
  - Victim Armed?

## Secondary [Census.gov]
- Mobile house rate
- Vehicle ownership rate
- Bachelor’s degree rate
- Median income
- Poverty rate

# Data prepping and tools
- Jupiter notebook and Python
- Custom columns: Month Year, year, Age Banding: under 10, 10-19, 20-29, etc.
- Using state name dataset to join multiple datasets

# Exploratory Data Analysis
Here is a high-level view of the shooting represented for all sates from 2015- 2021.

And here is the same data for shooting broken down by states.

And now we look at a table that breaks down this number by race and year. From the numbers below, it actually looks like white people were shot more than any other race. In fact, almost double that of black people.
This becomes more evident, when we look at it in a bar char that is grouped by race. For all the years, while people have been shot more than any other races.

Now let’s look at if the victims were armed when they were shot. From the table, below, it looks like on average, victims were not armed 90 % of the time.

Looking at the type of people they had, it was primarily gun or a knife. But we also see some interesting one like a hammer and a machete!

From another perspective, it looks like people in their 20s and 30s happen to be shot the most, followed by people in their 50s and then teens.
When we compare shooting by states, California, Texas and Florida seems to be the top 3 states.
Now let’s add in the secondary datasets to see if we find a correlation between the shooting and income level, education level, poverty rate, access to vehicle, mobile home rate. From the chart below, it doesn’t look like there is a similarity in the chart in the middle, that represents police shooting, and other socio-economic factors.
Let’s put them all in a correlation plot and see if we get a different result. However, doesn’t look like there is a strong correlation between the shotting count and the 5 socio economic factors.
Let’s plot all this information in a combination chart and see if we get a tend, in hopes of finding correlation. However, it doesn’t seem to be the case.

Now lets’s get population count by state and see if that helps explain any of this. As soon as we add the population dataset, we now see a strong correlation between shooting count and population. Almost close to +. This makes sense that where there are more people, there will be more shootings.

Similarly, in the combination chart, we see that the black line (population) closely follows the brown line (shooting count).
With that being said, let’s do a before an after comparison for the shooting count with the shooting count as is and calculate a per million count per race and see if we see a difference. This is important so that we remove the population distribution disparity by race and get a standardized rate.

Once we do so, it becomes evident that people of color are being impacted the most. Although in volume, while people have more instances because there are close to 4 times more white people than black in the US.
Similarly, once we do a before and after for the shooting count in a bar chart, it is really cleat that people of color are hurt more. This answers our first question that people of color are impacted the most by police shooting in the US.

# Forecasting
I used Facebook Prophet for my forecasting and with the data we have, it doesn’t look like the trending is going to change much. In fact, it is very similar to the historical data.

This makes sense because the shooting count has stayed pretty consistent around the 900s mark. However, for until August 2021, the count seems to be a third of the past years, so it is a little promising. 

# Obstacle
One of the obstacles I see for the shooting trend not tapering is because the use of body cams has stayed the same throughout the years. Maybe use of body cams would deter policemen from using appropriate level of action and not resolving to unnecessary shooting and violence.

# Summary
- Are people of color being impacted the most?
- Not at first glance. But Yes, black and Hispanic seem to be impacted the most.
- Are there any other socio-economic factors tied to shooting?
- Not really.
- How does the shooting trend will look like in the future?
- The trend seems to continue.










