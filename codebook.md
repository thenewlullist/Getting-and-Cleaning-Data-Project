#####This is a reference glossary of all the variables assigned in the run_analysis.R script


train.set <- reads table of training set

train.Y<- reads activity list of training set

sub.train<- reads the subject list of training set

test.set<- reads table of test set

test.Y<- reads activity list of test set

sub.test<- reads the subject list of test set

har.set<- joins the training set and test set

colnums<- extracts from a grep() command the column numbers of all categories that measure the mean or standard deviation

titles<- extracts from a grep() command the titles of all columns that measure the mean or standard deviation

full.set<- applies the column numbers as a subset of har.set, the joined train/test sets

activity<- coerce the train.Y$activity subset to a factor

tidy.set<- add the har.set[562] "activity" subset to the new tidy data set first so it will be the first column

means<- numeric vector of 556:561 which are the column numbers for the means measured in angle() 

tidy.names<- the column titles for the tidy data set 

gravityMean<- new column for the combined values of gravityMean X,Y and Z

tidy<- a subset of the other column titles to separate them from gravityMean

tidier<- command to arrange the new "tidy" variable data.frame by subject and activity for easier searching      

genlevels<- mixed numeric vector of the subjects who aren't missing (the only ones whose values were recorded in the angle() variables)
