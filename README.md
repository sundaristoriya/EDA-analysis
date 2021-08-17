# EDA-analysis
Car_evaluation
#importing lib
import pandas as pd
import numpy as np
import matplotlib as plot

#Read dataset
df=pd.read_csv("C:\\Users\\Welcome\\Desktop\\datasets\\car_evaluation.csv")

df

#shape will give the number of coulumns and rows (dimonsion of the dataset)
df.shape

#Head will help us to preview the dataset
df.head()

#Tail will give the last 5 items in the data set
df.tail()

#To find a columns
df.columns

#informaion of dataset
df.info

#we will name all the columns

Col_name=['buying', 'maint', 'doors', 'persons', 'lug_boot', 'safety', 'class']

df.columns=Col_name

Col_name

#after name columns we can preview the data with help of Head()

df.head()

# to check missing values we can use isnull()

df.isnull().sum()

# basic stats

df.describe()

#we can check the sample it will give random samples from dataset

df.sample(10)

# we will check he unique values in the data

Nunique=df.nunique()
Nunique

#we can sort the values 

Nunique=df.nunique()
Nunique=Nunique.sort_values()
Nunique

