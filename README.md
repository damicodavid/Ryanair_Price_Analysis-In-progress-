# **Welcome to Ryanair Price analysis in Python [IN PROGRESS]**

### *Characteristics:*
* Difficulty: _Beginner/Intermediate level_
* Program Language: _Python_
* Visualization Tool: _Tableau_

***

## 1.1 Scenario

<img src="https://github.com/damicodavid/Ryanair_Price_Analysis/assets/156213397/4ca23176-7a01-4bf6-901f-739855295eb5" alt="drawing" width="300"/>


Ryanair is an airline company founded in 1985 by Irish businessman Tony Ryan.
<br>
As of today, the company boasts *565 aircraft*, *over 22,000 employees*, and transported more than *142 million people in 2022*. 
<br>It operates over 3,000 routes daily across 40 countries and 240 airports.

We gathered data through an API of these 2 routes:
* Milano Maplpensa (MXP) --> Catania (CTA) - Sicily
* Milano-Bergamo (BGY) --> Catania (CTA) - Sicily

****

## 1.2 Goals Insights

1. How company discriminate the ticket price based on the starting airport (Main - Milano Malpensa, closer to the city & Secondary - Bergamo)

2. How does the ticket price change as we move further away from today's date and book with less advance notice??

3. How price differ from high to low season period (Ex: Christmas holidays)?


***
We'll analyze data from 01/11/2023 to 24/01/2023 and we'll present our insight through a interactive dashboard.

## 1.3 Step-by-step Analysis 

**1. Download the public data from -> [Datasets](xxxx)**

**2. Verify how is the data organized (columns structure and wideness)?**

**3. Are there issues with bias or credibility in this data?** 

**4. Does your data ROCCC (Reliable, Original, Comprehensive, Current, Cited)?**
<br>
<br>

**After these preliminary phases we can go through the _Data overview process_:**

**5.Install Packages on Python by Powershell Terminal:**

``` 
pip install numpy as np
pip install numpy pandas
pip install numpy matplotlib.pyplot
pip install numpy seaborn
``` 

**6.Import libraries & Overview your data:**

``` 
import pandas as pd

df = pd.read_excel('Ryanair_Data_300123.xlsx') 

df.head() # Quick check on how the dataset looks like
df.shape # Checking the shape of the data

```
This will give you and overview of your data:

![1 Overview Data](https://github.com/damicodavid/Ryanair_Price_Analysis-In-progress-/assets/156213397/37f93c89-eda2-4814-8643-1552cbed74bc)


**6. Check data type and other crucial info of each column:**

``` 
import pandas as pd

df = pd.read_csv("Divvy_Trips_2019_Q4.csv")
 
df.info() # Summary information about the dataframe

```
<br>
<br>

**After these overview phases we can go through the _Data manipulation and cleaning process_:**
<br>
**7.Check and remove any duplicates:**
```
import pandas as pd

df = pd.read_excel('Ryanair_Data_300123.xlsx') 

df.head() # Quick check on how the dataset looks like
df.shape # Checking the shape of the data
df.info() # Summary information about the dataframe
df.duplicated().sum() # Counting the duplicate rows
df.drop_duplicates(inplace=True) # Dropping the duplicate rows
df.to_csv('Ryanair_Data_300123_v1.csv', index=False)

```
<br>
<br>
<br>

Now we have all the data we need to start to analyse and create our dashboards that we will tell our story about the dataset in order to address our conclusions.

<br>
<br>

***
## 1.4 Visualization and Conclusions


Check my viz here->[Tableau Pubblic](xxx)
<br>
<br>
**INSIGHTS:**
1. xxx
2. xxx
3. xx

**SOLUTIONS:**
1. xxx
2. xxx
3. xxx
