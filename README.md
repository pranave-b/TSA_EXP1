### Developed by: Pranave B
### Register Number: 212221240040
### Date:

# Ex.No: 01A PLOT A TIME SERIES DATA

## AIM:

To develop a Python program that plots the time series data of Tesla's market price.

## ALGORITHM:

1. Import the required packages like pandas and matplotlib.
2. Read the dataset using pandas.
3. Convert the 'date' column to datetime format.
4. Plot the 'close' price against the 'date' column.
5. Label the axes and add a title to the plot.
6. Display the graph using plt.show().

   
## PROGRAM:

```
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('tesla_2014_2023.csv')
data.head()
data["date"]=pd.to_datetime(data["date"])
plt.plot(data['date'], data['close'], label='Time Series Data')
plt.xlabel('Date')
plt.ylabel('Price')
plt.title('Time Series Plot')
plt.legend()
plt.show(block=False)
plt.show()
```
## OUTPUT:

![exp1 img](https://github.com/user-attachments/assets/c69ca8fb-0f18-452f-9954-f72621303795)


## RESULT:

Thus to develop a python code that plots the time series data of Tesla's market price is successful.
