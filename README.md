(1) Data Description:
Provide a full descriptive summary of the dataset, including information such as the number of observations, number of variables, name and type of variables, what the variables mean, any issues you see in the data, any other potential issues related to things you cannot directly see, how the data were collected, etc. Make sure to use bullet point lists or tables to summarize the variables in an easy-to-understand format.

Note that the selected dataset will probably contain more variables than you need. In fact, exploring how the different variables in the dataset affect your model may be a crucial part of the project. You need to summarize the full data regardless of which variables you may choose to use later on.

We're mainly looking at the *player.csv* file. There are 9 variable columns, "experience", "subscribe", "hashedEmail", "played_hours", "name", "gender", "age", "individualId", "organizationName". 

- experience: A string that describes how much experience a player has had with Minecraft, you can be an Amateur, Regular, Pro, Veteran
- subscribe: A boolean that describes whether the player is subcribed to the mail or not
- hashedEmail: The player's email hashed to conceal their email infomation
- played_hours: The total hours this player has spent playing on the server
- name: The given name of the player based on the options on the website when you first register
- gender: The gender of the player, either Male, Female, Non-binary, Two Spirited, Prefer not to say, or Other
- age: The age of the player
- individualId: The id of the player, which is all NaN for now
- organizationName: The organization name of the player, which is all NaN for now

One clear issue we observed is the lack of data that was actually contributed by the player besides the hours spent on the game, which makes analysis all based on the total time spent by a player. 

(2) Question:
Clearly state one question your group will try to answer using the selected dataset. Your question should involve one response variable of interest and one or more explanatory variables. Describe clearly how the data will help you address the question of interest. You may need to describe how you plan to wrangle your data to get it into a form where you can apply one of the predictive methods from this class.

## Question 1: We would like to know which "kinds" of players are most likely to contribute a large amount of data so that we can target those players in our recruiting efforts. ##

Since we're looking at which kind of player are most likely to contribute to large amount of data. We need to look at the players experience, gender, age, subscribe, and compare it to the total hours spent on the game. For gender we'll look at the total hours spent by each gender, it will most likely be a histogram that has 4 sections with the mean time spent on the game for each gender. We can also use a histogram to plot the player experience against the average hour spent on the game. For age we can create a scatter plot plotting the age of the player against the time spent on the game. For subscribe since it's a boolean value, we can use a histogram as well and plot the average time played by a player who has subscribed versus a player who hasn't.

(3) Exploratory Data Analysis and Visualization
In this assignment, you will:

Demonstrate that the dataset can be loaded into Python.
Do the minimum necessary wrangling to turn your data into a tidy format. Do not do any additional wrangling here; that will happen later during the group project phase.
Make a few exploratory visualizations of the data to help you understand it.
Use our visualization best practices to make high-quality plots (make sure to include labels, titles, units of measurement, etc)
Explain any insights you gain from these plots that are relevant to address your question
Note: do not perform any predictive analysis here. We are asking for an exploration of the relevant variables to demonstrate that you understand them well before performing any additional modelling, and to identify potential problems you anticipate encountering.

(4) Methods and Plan
Propose one method to address your question of interest using the selected dataset and explain why it was chosen. Do not perform any modelling or present results at this stage. We are looking for high-level planning regarding model choice and justifying that choice.

In your explanation, respond to the following questions:

Why is this method appropriate?
Which assumptions are required, if any, to apply the method selected?
What are the potential limitations or weaknesses of the method selected?
How are you going to compare and select the model?
How are you going to process the data to apply the model? For example: Are you splitting the data? How? How many splits? What proportions will you use for the splits? At what stage will you split? Will there be a validation set? Will you use cross validation?

