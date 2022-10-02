Machine Learning Challenge - Alexander Powers

I completed to analysis models to try and predict the dispositions of various exoplanets.

For both models I cleaned the data by dropping columns featuring NA, columns with values too large for their data type, rows containing NA values as well as columns containing strings except for 'koi_disposition', which I used as the y axis of my analysis.

After splitting the data into text and train categories, I further prepared the data by using LabelEncoder for the y axis, and StandardScaler for the x axis.

For the first model I used Support Vector Machine. The initial score for the model was 88.77%. I ran a GridSearchCV to find a more accurate result, however after tweaking the parameters based off the GridSearch's best_params_ function, the accuracy of the model was 88.52%, pretty much the same as before.

My second model used the KNeighborsClassifier. After running various outcomes through a for loop, I made a decision that k number 9 was the most accurate and achieved a score of 83.39%. The GridSearchCV found k number 29 to be the most accurate and produced a similar score of 82.63%, which was actually a slight bit worse than my choice.

