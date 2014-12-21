Original Data

Conventions followed

Processing code and dataset variable naming follows the conventions described in Google R Styde Guide.

Data sets

Raw data set

The raw dataset was created using the following regular expression to filter out required features, eg. the measurements on the mean and standard deviation for each measurement from the original feature vector set

-(mean|std)\\(

This regular expression selects 66 features from the original data set. Combined with subject identifiers subject and activity labels label, this makes up the 68 variables of the processed raw data set.

The training and test subsets of the original dataset were combined to produce final raw dataset.

Tidy data set

Tidy data set contains the average of all feature standard deviation and mean values of the raw dataset. Original variable names were modified in the follonwing way:

Replaced -mean with Mean
Replaced -std with Std
Removed parenthesis -()
Replaced BodyBody with Body
