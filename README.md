# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 12-08-2025
### Name:  GEDIPUDI DARSHANI

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```p
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('india.csv')
df.shape

df1=df.head(100)
df1
```
<img width="1134" height="519" alt="image" src="https://github.com/user-attachments/assets/44864c78-0efe-4941-8a7a-b70f207d7cf3" />

```p
df.info()
```
<img width="933" height="367" alt="image" src="https://github.com/user-attachments/assets/ad2b2f98-5d30-403f-896c-9feeea3408df" />


```
df.describe
```
<img width="1061" height="440" alt="image" src="https://github.com/user-attachments/assets/15c648d3-c73d-4157-bb91-493b129be8b3" />


```p
x=df1['date']
y=df1['open']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('Date vs Open')
plt.xlabel('Date')
plt.ylabel('Open')
plt.show()
```

# OUTPUT:
<img width="1315" height="699" alt="image" src="https://github.com/user-attachments/assets/63407615-e112-4d4d-9595-f53c081c25c3" />


It is stationary data.

# RESULT:
Thus we have created the python code for plotting the time series of given data.
