# San Franco Crime Analysis/Prediction

Below is pasted from the kaggle page:

From 1934 to 1963, San Francisco was infamous for housing some of the world's most notorious criminals on the inescapable island of Alcatraz.

Today, the city is known more for its tech scene than its criminal past. But, with rising wealth inequality, housing shortages, and a proliferation of expensive digital toys riding BART to work, there is no scarcity of crime in the city by the bay.

From Sunset to SOMA, and Marina to Excelsior, this competition's dataset provides nearly 12 years of crime reports from across all of San Francisco's neighborhoods. Given time and location, you must predict the category of crime that occurred.

We're also encouraging you to explore the dataset visually. What can we learn about the city through visualizations like this Top Crimes Map? The top most up-voted scripts from this competition will receive official Kaggle swag as prizes. 

-- End Paste


So we are trying to predict the category of a crime, given the time and location. We are given nine columns of data:

- Dates - timestamp of the crime incident
- Category - category of the crime incident (only in train.csv). This is the target variable you are going to predict.
- Descript - detailed description of the crime incident (only in train.csv)
- DayOfWeek - the day of the week
- PdDistrict - name of the Police Department District
- Resolution - how the crime incident was resolved (only in train.csv)
- Address - the approximate street address of the crime incident 
- X - Longitude
- Y - Latitude

That seems really elementray so maybe we can try to see if there are more serious crimes depending on the location. That woud require some other techniques that will require some more time spend on. But it can be done, I would also like to see if I can make a bayesian model and compare it to the frequentist version. Since that can get us some more brownie points, and better grade, I don't know though.
There are isn't much to go off of when it comes to data, yes I know there could be hundres of thousands of rows. But the features aren't much to work off of since there is a lot that goes into predicting time. Plus some of the more interesting things we could potentionally find aren't even in here. So thats a bummer but it's what ever.

Models that will be used (Or may not be used IDK yet):

- Support Vecoter Machine
- Multiple Logistic Regression
- Random Forest
- XGBoosted Random Forest
- kNN (Maybe? Will need something more robust)
- Bayesian Multiple Logistic Regression
- Bayesian Random effects Model?

Feature Engineering Stuff:
- **More to come**
- *Cyclic Encoding*

As for libraries we are using:
- Polars
- numpy
- Sklearn
- Seabron (with matplotlib)
- scikit-learn
- pyro
- *More will some since pyro needs more than one library*


# TODO
John:
- cross validation for all the freqentist model
- better model metrics : accuracy, precision, recall, the F1 score, and the confusion matrix (I kindaalready added this it just needs to be better outputted so that we can just paste into latex
- hyper parameter tuning
- Do the xgboosted Random Forest

Michael:
- Bayesian Logistic Regression
- BART Model
- Bayesian heirarcheliel model
- Then model statistics for this stuff

Together:
Once we are done hopefully by the 5th of Nov, we will start the presentation making process and making the paper since.
Sine we are kinda doing a lot we need to be detailed in the paper but I think this will be good pracice for anyother future stuff we do.






