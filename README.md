# Predicting NFL Playoff Outcomes: A Data Analytics Journey in Databricks
A personal project combining my love for football with hands-on data analysis

## The Challenge
As a 10-year NFL fan (fly Eagles fly!) I've always enjoyed watching games casually, following my team, catching the Super Bowl, and playing fantasy football. But this year, when the Eagles bowed out early in the playoffs, I was curious and decided to take a different approach: Could I use data to predict which teams would advance?

**I set out to analyze playoff teams by comparing their offensive, defensive, and quarterback performance throughout the season**. My goal was twofold: understand what makes winning teams tick, and explore what I could accomplish using Databricks' free edition.

Due to Databricks limiting public access I created a replica of the [Dashboard](https://public.tableau.com/app/profile/lynn.lennmor/viz/NFLPlayoffPicture/NFL_Payoff_Picture) in Tableau for anyone to interact with.


## The Objective
Core Question: Can season-long statistics predict playoff progression?

I focused on key metrics:

- Win/loss records (regular season & postseason)

- Offensive and defensive yards (average per game)

- Quarterback passing yards and completion percentages

**Technical Goal:** Build an end-to-end analytics workflow in Databricks, from data ingestion to dashboard creation.


## My Approach

### 1. Data Collection
I leveraged a data pipeline I'd built in an earlier NFL project (saving me significant setup time). Using Python, I gathered the necessary data and transferred it to SQL, then imported CSV files into Databricks.

### 2. Question Framework
I developed four analytical questions to guide my analysis:

Q1: What are the win/loss rates of each playoff team? Purpose: Establish baseline team performance

Q2: What are each team's offensive & defensive yards (total and per game)? Purpose: Identify team strengths and potential matchup advantages

Q3: What is each QB's passing yard performance? Purpose: Assess quarterback impact on team success

Q4: What is each QB's completion percentage? Purpose: Evaluate passing efficiency and consistency

[Link to all queries](https://github.com/lynnlennmor/NFL-Playoff-Picture/blob/main/NFL%20Playoffs%20Analysis.ipynb)

## 3. Dashboard Design
I structured the dashboard as an analytical funnel:

- Top Level: Win/loss overview

- Mid Level: Offensive/defensive stats with filtering capabilities

- Detail Level: QB-specific metrics with semi-filtering

All queries were written in SQL within Databricks notebooks, making it easy to iterate and refine visualizations.

## Analytical Insights:
While the data alone wasn't sufficient for precise predictions, it provided valuable directional insights:

- Top-performing regular season teams generally progressed further in the playoffs (Ex:Patriots, Broncos, Seahawks and Rams made it to Conference)

- Strong regular season defense/offense didn't predict early playoff success, but became a bit more influential in the conference games - as did overall QB accuracy


## Key Learnings & Results
What I Achieved:

- ✅ A comprehensive dashboard visualizing playoff team performance across regular and postseason

- ✅ Hands-on experience with Databricks' SQL interface, notebooks, and dashboard creation 

- ✅ Deeper understanding of NFL statistics and how they're calculated (like defensive yards)


## Technical Takeaways:
Pros of Databricks:

- Seamless SQL integration made query adjustments effortless

- Dashboard creation was intuitive and fast

Cons/Considerations:

- Easy editing can lead to over-optimization (constantly tweaking instead of finishing!)

- Required critical thinking about which metrics truly complement each other

## Future Enhancements
This project opened up several exciting possibilities:

Data Expansion:

- Add rushing yards to better assess offensive versatility against different defenses

- Include turnover ratios and red zone efficiency

- Incorporate injury reports and weather conditions

Automation:

- Connect Databricks to live data sources for real-time updates

- Build automated weekly reports throughout future season

- Set up alerts for significant statistical changes

## Final Thoughts
This project reminded me that sometimes the best learning happens when you combine something you're passionate about with a skill you want to develop. This is exactly what I'm trying to do, simply learn and develop while exploring something that I think is fun.

### Tools & Duration:
| Category      | Tools                                                           |
| ------------- | --------------------------------------------------------------- |
| Programming   | Python, SQL                                                     |
| Data Source   | [NFLReadPy](https://nflreadpy.nflverse.com/api/load_functions/) |
| Database      | Databricks                                                      |
| Visualization | Tableau, Databricks                                             |
| Duration      | ~ 1 week                                                        |


