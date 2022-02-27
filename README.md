# Final-Project

## The economic impact of COVID across people in different demographic groups and education levels.

## Introduction
COVID has had a huge impact on the economy and our lives. The impact of COVID has not been uniform across different groups. By conducting this study, we hope to examine how COVID has affected individuals in terms of their employment situation. Findings from this study could help policy makers in creating appropriate support structures for affected individuals. For this study, we have narrowed our focus to North Carolina. 

## Data Source
The data for this project has been downloaded from Integrated Public Use Microdata Series (IPUMS)[1] which is the world's largest individual-level population database.
[IPUMS](https://en.wikipedia.org/wiki/IPUMS)
The data itself is from the American Community Survey (ACS) which is a demographics survey program conducted by the U.S. Census Bureau.
[ACS](https://en.wikipedia.org/wiki/American_Community_Survey)

## Purpose
The primary question that this project aims to answer is:

What are the demographic and educational attainment factors that predict who is able to work in North Carolina even during a pandemic?

## Machine Learning Model
### Description of Preprocessing
<Vedika - please feel free to update this section - thanks, Timothy>
Our initial dataset (filename: Data_Cleaning/demogrphic_data_NC.csv) was created from a raw file, which was pared down to show only North Carolina data. The data was read into a Jupyter Notebook and Pandas was used to created a DataFrame whilst dropping some columns.  The rows of this dataset were cleaned to drop records with "99" values, aka, bad data.  This dataset included only number values, which corresponded to text values; data was cleaned to show the corresponding text values instead of the coded numbers, so that the data would make sense to a person reading it.  Data was mapped for: Sex, Education Level, Race, and Marital Status.  

### Machine Learning part 1
The above mentioned variables - Sex, Education Level, Race, and Marital Status - were selected as features, and 'COVIDUNAW' was selected as the target.  The COVIDUNAW field was an indicator of whether or not the person was able to work.  
First (filename: Machine_Learning/CCMachineLearning3.ipynb), we attempted to use a simple straightforward Supervised Learning Model from the SciKit Learn (sklearn) library.  To prepare our data for this, we employed the Pandas get_dummies() method. Then, we split our data into Training and Testing sets by using the train_test_split method from the sklearn library.  Using another method from sklearn library, StandardScaler, we scaled the data values and had the Model make predictions.  
Once we had those results, we created a confusion matrix and accuracy score.

### ML_Model_1 Results
The confusion matrix that we created was saved down to a csv file (filename: Machine_Learning/confusionmatrix1.csv)

### Machine Learning part 2

### ML_Model_2 Results

## Communication Protocols
Team Members:

Chris Capps

Timothy Keating

Vedika Nigam

Abazar Rahma

This group will meet during class time on Tuesdays and Thursday; as well as on Mondays and Wednesdays at 7pm on Zoom. Group members are in contact via email, mobile phone and Slack. Team members have their GitHubs set up with each team member owning a branch off of 'main'.

## References: 

[1] Sarah Flood, Miriam King, Renae Rodgers, Steven Ruggles, J. Robert Warren and Michael Westberry. Integrated Public Use Microdata Series, Current Population Survey: Version 9.0 [dataset]. Minneapolis, MN: IPUMS, 2021. https://doi.org/10.18128/D030.V9.0



## Who Did What - Segment #1
Timothy: 
- Worked on setting up the GitHub
- pgAdmin DB
- I assisted in the Machine Learning Model setup.  

Chris:  
- Machine Learning 

Vedika:
- README file
- Data Cleaning in Python

Abazer:
- Data Cleaning in Python
- Machine Learning
