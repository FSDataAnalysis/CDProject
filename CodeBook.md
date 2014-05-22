# RELEVANT DATA SETS 

  The following are data sets that the file run_analysis.R produces from the
  data [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
  
* merged_data   
	
  The merged_data data set contains the training and test data sets 

* data_Set_mean_std

  The data_Set_mean_std data set contains the data set with mean and standard
  values only

* labled_activities

  The labled_activities data set contain descriptive activity names: 
		
  walking, walkingupstairs, walkingdownstairs, sitting, standing, laying

* labeled_data_set

  The labeled data set containes the names (column names or labels) of the 
  variables with descriptive names in lower case. 

* Tidy_Data_Set

  The tidy data set is the result of averaging for every subject and for 
  activity, i.e 30 subjects each of one has 6 rows according to activity. 
  Activities and subjects are described in the README.md file. 


# VARIABLES

## Variables list

|    | Variables                         |
|----|-----------------------------------|
| 1  | subject                           |
| 2  | activity                          |
| 3  | tbodyaccmeanx                     |
| 4  | tbodyaccmeany                     |
| 5  | tbodyaccmeanz                     |
| 6  | tgravityaccmeanx                  |
| 7  | tgravityaccmeany                  |
| 8  | tgravityaccmeanz                  |
| 9  | tbodyaccjerkmeanx                 |
| 10 | tbodyaccjerkmeany                 |
| 11 | tbodyaccjerkmeanz                 |
| 12 | tbodygyromeanx                    |
| 13 | tbodygyromeany                    |
| 14 | tbodygyromeanz                    |
| 15 | tbodygyrojerkmeanx                |
| 16 | tbodygyrojerkmeany                |
| 17 | tbodygyrojerkmeanz                |
| 18 | tbodyaccmagmean                   |
| 19 | tgravityaccmagmean                |
| 20 | tbodyaccjerkmagmean               |
| 21 | tbodygyromagmean                  |
| 22 | tbodygyrojerkmagmean              |
| 23 | fbodyaccmeanx                     |
| 24 | fbodyaccmeany                     |
| 25 | fbodyaccmeanz                     |
| 26 | fbodyaccmeanfreqx                 |
| 27 | fbodyaccmeanfreqy                 |
| 28 | fbodyaccmeanfreqz                 |
| 29 | fbodyaccjerkmeanx                 |
| 30 | fbodyaccjerkmeany                 |
| 31 | fbodyaccjerkmeanz                 |
| 32 | fbodyaccjerkmeanfreqx             |
| 33 | fbodyaccjerkmeanfreqy             |
| 34 | fbodyaccjerkmeanfreqz             |
| 35 | fbodygyromeanx                    |
| 36 | fbodygyromeany                    |
| 37 | fbodygyromeanz                    |
| 38 | fbodygyromeanfreqx                |
| 39 | fbodygyromeanfreqy                |
| 40 | fbodygyromeanfreqz                |
| 41 | fbodyaccmagmean                   |
| 42 | fbodyaccmagmeanfreq               |
| 43 | fbodybodyaccjerkmagmean           |
| 44 | fbodybodyaccjerkmagmeanfreq       |
| 45 | fbodybodygyromagmean              |
| 46 | fbodybodygyromagmeanfreq          |
| 47 | fbodybodygyrojerkmagmean          |
| 48 | fbodybodygyrojerkmagmeanfreq      |
| 49 | angletbodyaccmeangravity          |
| 50 | angletbodyaccjerkmeangravitymean  |
| 51 | angletbodygyromeangravitymean     |
| 52 | angletbodygyrojerkmeangravitymean |
| 53 | anglexgravitymean                 |
| 54 | angleygravitymean                 |
| 55 | anglezgravitymean                 |
| 56 | tbodyaccstdx                      |
| 57 | tbodyaccstdy                      |
| 58 | tbodyaccstdz                      |
| 59 | tgravityaccstdx                   |
| 60 | tgravityaccstdy                   |
| 61 | tgravityaccstdz                   |
| 62 | tbodyaccjerkstdx                  |
| 63 | tbodyaccjerkstdy                  |
| 64 | tbodyaccjerkstdz                  |
| 65 | tbodygyrostdx                     |
| 66 | tbodygyrostdy                     |
| 67 | tbodygyrostdz                     |
| 68 | tbodygyrojerkstdx                 |
| 69 | tbodygyrojerkstdy                 |
| 70 | tbodygyrojerkstdz                 |
| 71 | tbodyaccmagstd                    |
| 72 | tgravityaccmagstd                 |
| 73 | tbodyaccjerkmagstd                |
| 74 | tbodygyromagstd                   |
| 75 | tbodygyrojerkmagstd               |
| 76 | fbodyaccstdx                      |
| 77 | fbodyaccstdy                      |
| 78 | fbodyaccstdz                      |
| 79 | fbodyaccjerkstdx                  |
| 80 | fbodyaccjerkstdy                  |
| 81 | fbodyaccjerkstdz                  |
| 82 | fbodygyrostdx                     |
| 83 | fbodygyrostdy                     |
| 84 | fbodygyrostdz                     |
| 85 | fbodyaccmagstd                    |
| 86 | fbodybodyaccjerkmagstd            |
| 87 | fbodybodygyromagstd               |
| 88 | fbodybodygyrojerkmagstd           |

## Description of Variables

* subject 

The subject variable is found as the first column of the tidy data set (Tidy_Data_Set) and it stands for the subject that carried out the experiment. The range is 30, i.e. 1-30. The unit is person. 

* activity 

The activity variable is a descriptive variable (no units) found as the second column of the tidy data set. It stands for walking, walkingupstairs, walkingdownstairs, sitting, standing, laying in order and for each subject. This describes how the experimets where performed by the subjects.

* rest of variables

1. Too many to describe. I will not describe it here since it is a waste I think but one can find the description as given by the  [files](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) given in the project. 

2. A good point is to mention the values have been  normalized and bounded within [-1,1] interval. 

3. The raw was obtained as accelerations and mean and standard devitions were calculated. 

4. The FFT transform was applied and the resulting set is given with a t in the front or an f according to whether they relate to the time of frequency domains (first character of the variable name).  

5. The variables can also refer to the x, y or z axes and the lables (names) have an x, y or z accordingly when required. 

6. Whether a variable stands for mean or standard devation can also be inferred from their name as mean or std. 






