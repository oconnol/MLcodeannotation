# MLcodeannotation

## Ultimate function
- takes in a start and end time as inputs
- takes these times and creates a dataframe containing all of the trip locations and the dates of trips
- creates a list of dataframes and plots, one for each trip time and location, contains data from significant PVs 5 minutes before and 10 seconds after trip time
- creates another list of dataframes and plots for raw data unadjusted for time
- uses the data specific to CB cavities and creates a single dataframe where each row is a different trip event and the columns represent the mean, standard deviation, max, min, 1st quartile, and 3rd quartile for each PV within the cavity
- imports a premade dataframe containing a training set
- this training set is used to fit an XGBClassifier model
- the model is then used to predict the trip type for all the cavities within the large CB dataframe
- the model predictions are translated to their proper labels and the function returns a dataframe containing the trip event data and their labels
