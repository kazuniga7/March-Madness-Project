# March-Madness-Project
# This program was a partner project where my partner and I tested different models to see which
# would best be suited to predict the 2025 March Madness bracket based on the match-up difference of regular season team
# stats of that year.
# The code marked "Kevin code" was work done by me, and the work marked "Mack code" was done by my partner.


# Model Training:
# The models were always trained on the results of the previous years' March Madness and the previous year's only because
# our personal opinion was that using data from later years isn't as reasonable since teams, coaching, and other factors change.
# We evaluated each model based on how well it predicted the 2024 March Madness matchups when trained on the 2023 March Madness data.
# We trained a total of 4 different models where we first tried tuning the input features then hyperparameters, and then doing the
# it the other way around. In addition,we ensembled each pairing. I worked with KNeighbors and GaussianNB models and my partner
# worked with LogisticRegression and RandomForestClassifier models.
# The base input features we decided to start with were a personal decision made by my partner who had more 
# knowledge of basketball than me.


# Data Collection:
# We scraped data off two websites, the NCAA website and the College Basketball Sports Reference website. From the NCAA website,
# we got the 2023 and 2024 March Madness matchups and seedings. From the Sports Reference website, we got the regular season
# stats for the teams in each year.
# I web-scraped the NCAA website while my partner scrapped the Sports Reference website. My partner then combined all the scraped data
# into one data frame containing the matchups for March Madness and the difference in team stats based on the matchups.


# Results:
# After comparing the statistics of each model, specifically the f1 scores, the model that performed the best was the Random Forest
# ensemble model we tested. The runner up to this model was one of the GaussianNB models we also tested. Although statistically these
# models tested well, my partner and I still came to the conclusion that the March Madness tournament is something that is very difficult
# to predict. My partner who knows more about basketball then me was a little unsure of some of the predictions that both models outputed.
# Below are the predicted brackets of each model.

# Of the code below, the starting code is the web scraping used to obtain all the data. The code that follows is easy access to the
# predictions outputted by the GaussianNB and RandomForest ensemble model spoken of above for comparison.
# The rest of the code that follows after is all the testing that was done with different models.
