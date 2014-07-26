# Getting and Cleaning Data: Course Project

This project includes a script called `run_analysis.R` which can be ran against the dataset that is available [here](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip). A full description of this data can be found [here](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones).

## About the raw data
The features (561 of them) are unlabeled and can be found in the x_test.txt. 
The activity labels are in the y_test.txt file.
The test subjects are in the subject_test.txt file.

The same holds for the training set.

## About the script and the tidy dataset
The script `run_analysis.R` which will merge the test and training sets together and create a tidy dataset `tidt.txt`

### Prerequisites for this script:
1. The dataset must be downloaded and extracted
2. the UCI HAR Dataset must be availble in a folder called `UCI_HAR_Dataset`

After merging testing and training, labels are added and only columns that have to do with mean and standard deviation are kept.

Lastly, the script will create a tidy data set containing the means of all the columns per test subject and per activity.

This tidy dataset will be written to a tab-delimited file called `tidy.txt`

## Code Book
The `CodeBook.md` file explains the transformations performed and the resulting data and variables.

## Repository Information
`.gitignore` will not add the `UCI_HAR_DATASET` nor the `tidy.txt` back to the repository.