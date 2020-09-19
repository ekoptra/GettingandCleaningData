# Getting and Cleaning Data
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. Here are the data for the project: [Data](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)

# Code Explanations
I used `dplyr` library for this project
```r
install.packages("dplyr")
library(dplyr)
```

I applied all same read format to the files. I used `sep=""` cause given file format seperated like that. And also `header=FALSE`, just dont want to lose first row of data. If its true, first row would be column names which I don't want to.

Read features and Activity: 
```r
features <- read.csv("features.txt", header = FALSE, sep = "")[2]
activity <- read.csv("activity_labels.txt", header = FALSE, sep = "")
```

Read X test and training data:
```r
train_data <- read.csv("train/X_train.txt", sep="", header = FALSE)
test_data <- read.csv("test/X_test.txt", sep="", header = FALSE)
full_data <- rbind(train_set, test_set)
```

Read subject who performed the activity:
```r
train_person <- read.csv("train/subject_train.txt", sep="", header = FALSE)
test_person <- read.csv("test/subject_test.txt", sep="", header = FALSE)
full_person <- rbind(train_person, test_person)
```

Read activity for subject
```r
train_activity <- read.csv("train/y_train.txt", sep="", header = FALSE)
test_activity <- read.csv("test/y_test.txt", sep="", header = FALSE)
full_activity <- rbind(train_activity, test_activity)
```

Assign variabel name and extracts the measurements on the mean and standard deviation:
```r
names(full_data) <- features[,1]
mean_std_data <- full_data[grepl("std|mean", names(full_data), ignore.case = TRUE)]
```

Merge PersonID, Person's activity, and all data:
```r
full_activity <- (merge(full_activity, activity, by="V1"))[,2]
full_activity <- cbind(full_person, full_activity)
names(full_activity) <- c("PersonID", "Activity")
mean_std_data <- cbind(full_activity,mean_std_data)
```

Tidy data set with the average of each variable for each activity and each subject:
```r
tidyData <- mean_std_data %>% 
                group_by(PersonID, Activity) %>%
                summarise_each(funs(mean))
```
