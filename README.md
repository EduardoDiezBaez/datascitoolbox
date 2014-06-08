---
title: "Getting and Cleaning Data - Peer Project"
author: "Eduardo Díez"
date: "Sunday, June 08, 2014"
output: html_document
---
datascitoolbox - Getting and Cleaning Data
==============

The Data Scientist’s Toolbox by Jeff Leek course from COURSERA

By student Eduardo Díez Báez


## A little explanation about the script 'run_analysis.R'


Follow a summary of the steps the scrip follow to get the datasets files required.
Aditional the script itsel is full documented



  Let's state our root working directory where scripts and datasets are
 
 
  We read the file 'feature.txt' to get the 561 variables' names that correspond
  to each variable at both 'X_???.txt' files (test and train).
  The so obtained table have two columns; 
  the first with sequential integers from 1 to 561 and the second the variables names  
 
 
  we assing to both columns a more convenient and descriptive names
 
 
  We keep all 561 variables in a char variable called 'mynames'
 
 
  Now, we extract the columns position --number-- that correspond with 
  the measurements on the mean and standard deviation of measurements only 
  and we save them in 'ColMean' and 'ColStd' and 'ColTotal'
 
 
  We add to ColTotal the three first columns that are going to be myID, myOrgFile, volunter, activity
 
 
  Now, we open each set of data file, three for 'test' and another three for 'train'  
  and we add the same variable 'myID' to each set (X_???.txt; subject_???.txt and y_???.txt).
  'myID' will be filled with a sequentia from 1 to length of each datafile and we are going
  to use it to help us to join the data, in such a way that every dataset have 
  the subjects (numbers from 1 to 30 that correspond toeach 30 volunteers) and 
  the activity (from 1 to 6). 
  In our case the amount of rows of all of them is 2947 rows
  
 
  we change the columns names of X_???.txt for our descriptive ones
 
 
 
 
  Finally we take out the columns we don't need, including the three we added above
 
  We repeate the same last procedure for the 'train' files
 
 
 
  Now, we need join both datasets
 
 
  And, we write down descriptive activity names to name the activities in the dataset
 
  
 
  The first submission dataset file should be as 'my_data' but withouth the first three columns;
  with only the measurements on the mean and standard deviation for each measurement.
 
 

