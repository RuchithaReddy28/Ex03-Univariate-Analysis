## Ex03-Univariate-Analysis
## AIM
To read the given data and perform the univariate analysis with different types of plots.

##  EXPLANATION
Univariate analysis is basically the simplest form to analyze data.Uni means one and this means that the data has only one kind of variable.The major reason for univariate analysis is to use the data to describe.The analysis will take data,summarise it,and then find some pattern in the data.
## ALGORITHM
# STEP 1
Read the given data.
# STEP 2
Get the information about the data.
# STEP 3
Remove the null values from the data.
# STEP 4
Mention the datatypes from the data.
# STEP 5
Count the values from the data.
# STEP 6
Do plots like boxplots ,countplots,distribution plot,histogram plot.

## PROGRAM
```
Developed by:Akkireddy Ruchitha Reddy
Registration Number:212221230004
```
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
## OUTPUT
# DATA
!
# DATA HEAD
!
# DATA INFORMATION
!
# DATA DESCRIBE
!
# DATA NULL VALUES
!
# DATA'S DATATYPES
!
# DATA'S VALUECOUNT
!
# BOXPLOT
!
# COUNTPLOT
!
# DISTRIBUTION PLOT
!
# HISTOGRAM PLOT
!

## RESULT
Thus we have read the given data and performed the univariate analysis with different types of plots.
