# Day-1

Data is a collection of raw facts and figures that have no meaning by themselves.

Information is processed and organized data that has meaning and is useful for decision-making.

 
example: we have to maintain weekly information of road accidents we collect raw data from newspapers etc 
now i have to maintain monthly info so that weekly info becomes my data 

Outliers are values that are very different from the other values in a dataset.

Structured data is data that is organized in rows and columns and stored in databases or spreadsheets.

Unstructured data is data that does not have a fixed format or structure.

Primary data is data collected directly by the researcher for a specific purpose.

Secondary data is data that has already been collected by someone else and is used for research.





# Day-2
Python is dynamically based understand we dont need to initialise any variable

age=29
print(type(age))
Output: int

Data structure in python:

List- ordered and mutable

marks=[10,20,30]

tuple-ordered and immutable 

months=('jan','feb','march')

dictionary-unordered and mutable.Keys must be unique and immutable

user={'name':'Alex','age':20}

for specific value

print(user['name'])

set-unordered and duplicate eliminate.{} ()

ids={101,102,101}
print(ids)

output:101,102

pandas-library that is used for data manipulation and analysis

import pandas as pd





# Day-3
how to handle data

understand the data 

data cleaning  

in data cleaning we clean redundant and missing values 

Regex- regular expression 

functions of pandas of data cleaning :

method to handle missing values:

df.dropna()  used to drop full row thatvcontain null value 

we can add mean mode median instead of missing or null values 

fill mean when numerical content is there 

fill mode when categorial content is there

now how to handle duplicate rows 
df.duplicated (if it returns true value for any column it means we have duplicate values 
 
 we can drop it by df=df.drop_duplicates()

  next is to standardize the data it means we have same value but with different spellings they consider it differently 

  df["Gender"]=df['Gender'].str.title()

df['Name']=df['Name'].str.strip() //to remove the extra spaces 

Outliers 
it means some values are out of range or graph IQR method is mathematical way to handle it 

after applying all the updations we can save the new cleaned dataset into drive so that no dataset will loss 





#Day-4

EDA - exploratory data analytics 

now after cleaning the dataset next is to analysis the dataset that how many rows and columns are there which values a column contain 

df.shape is used to take the rows and cols of the dataset 

df['dept'].unique() is used to identify the values of the dept 

if we enter nunique then it gives us numeric value of how many values can a column contain 

df['dept'].value_counts() is use to identify that different dept contain how many values 

in analysis we use univariate,bivariate and multivariate  

in univariate we have one single col we can apply mean mode median min max into that 

in bivariate we have one col correspond to one column 

in multivariate one col correspondence to another columnss

crosstab is replace with group by it make tabular and frequency distribution table it is also one col to one col 

corr is also multivariate 

corr= df.corr(numeric_only=True) 

1.0 means perfect +ve correlation 

-1.0 means perfect -ve correlation 

0.0 means no linear correlation 

sorting can also be done by df.sort_values(by='CGPA',Ascending=False) by default ascending is true 

Feature engineering 

in this we have one col on basis of that we create another column 
df['excellent']=df['cgpa']>=9

this will create column excellent with true and false values 
