# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import matplotlib.pyplot as plt
#create data for plotting
x_values = [0, 1, 2, 3, 4, 5] 
y_values = [0,1,4,9,16,25]
#the default graph style for plot is a line
plt.plot(x_values, y_values)
#display the graph
plt.show()
```


<img width="717" height="495" alt="image" src="https://github.com/user-attachments/assets/09650d3e-7bda-4328-8c7a-0cbe2626c4c1" />


```
# importing the required module
import matplotlib.pyplot as plt

# x axis values
x = [1, 2, 3]
# corresponding y axis values
y = [2, 4, 1]

# plotting the points
plt.plot(x, y)

# naming the x axis
plt.xlabel('x - axis')
# naming the y axis
plt.ylabel('y - axis')

# giving a title to my graph
plt.title('My first graph!')

# function to show the plot
plt.show()
```


<img width="665" height="537" alt="image" src="https://github.com/user-attachments/assets/af4c7a60-8c87-4089-a4db-a8d1f859ed16" />



```
import matplotlib.pyplot as plt
# line 1 points
x1 = [1, 2, 3]
y1 = [2, 4, 1]
# plotting the line 1 points
plt.plot(x1, y1, label="line 1")
# line 2 points
x2 = [1, 2, 3]
y2 = [4, 1, 3]
# plotting the line 2 points
plt.plot(x2, y2, label = "line 2")
# naming the x axis
plt.xlabel('x axis') 
# naming the y axis
plt.ylabel('y axis')
# giving a title to my graph
plt.title('Two lines on same graph!')
# show a legend on the plot
plt.legend()
# function to show the plot
plt.show()
```


<img width="712" height="551" alt="image" src="https://github.com/user-attachments/assets/1534fb7e-4761-4f4f-9760-a9b7d8fcd702" />


```
import matplotlib.pyplot as plt

#x axis values
x = [1, 2, 3, 4, 5, 6]
# corresponding y axis values
y = [2, 4, 1, 5, 2, 6]
# plotting the points
plt.plot(x, y, color='green', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='blue', markersize=12)
# setting x and y axis range
plt.ylim (1,8)
plt.xlim (1,8)
# naming the x axis
plt.xlabel('x -axis')
# naming the y axis
plt.ylabel('y axis')
#giving a title to my graph
plt.title('Some cool customizations!')
# function to show the plot
plt.show()
```


<img width="702" height="532" alt="image" src="https://github.com/user-attachments/assets/fe431f99-03de-4ea6-8b32-3e50fbfba7f0" />


```
years=range(2000, 2012)
apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ]

plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges']);
```


<img width="731" height="542" alt="image" src="https://github.com/user-attachments/assets/ee25381b-e9d6-4bd1-974c-c9f46268db2e" />


```
import matplotlib.pyplot as plt
# x-axis values
x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
# y-axis values
y = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]
# plotting points as a scatter plot
plt.scatter(x, y, label= "stars", color="green", marker="*", s = 30 )
# x-axis label
plt.xlabel('x - axis')
# frequency label
plt.ylabel('y -axis')
# plot title
plt.title('My scatter plot!')
# showing legend
plt.legend()
# function to show the plot
plt.show()
```


<img width="726" height="545" alt="image" src="https://github.com/user-attachments/assets/c1aa88c1-3ac0-4536-a725-2ac87ae83ea8" />


```
#Compute the x and y coordinates for points on a sine curve
x = np.arange(0, 4*np.pi, 0.1)
y = np.sin(x)
plt.title("sine wave form")
#Plot the points using matplotlib
plt.plot(x, y)
plt.show()
```


<img width="762" height="525" alt="image" src="https://github.com/user-attachments/assets/05421b28-477a-45ab-9c63-3b8866f4b766" />


```
import matplotlib.pyplot as plt
import numpy as np
# Create some random data
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
# Create the plot
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','2'])
plt.show()
```

<img width="701" height="472" alt="image" src="https://github.com/user-attachments/assets/f22bc39c-97a9-4b96-8ace-294a3577a1ce" />


```
plt.stackplot(x, y1, y2, y3, labels=['Line 1', 'Line 2', 'Line 3'])
plt.legend(loc='upper left')

plt.title('Stacked Line Chart')

plt.xlabel('X-axis')

plt.ylabel('Y-axis')

plt.show()
```

<img width="695" height="532" alt="image" src="https://github.com/user-attachments/assets/6613258c-9f9e-439b-b0bd-e17d0b8d5b6c" />


```
# define new x values for spline line
x_smooth = np.linspace(x.min(), x.max(), 100)
# create spline line
y_smooth = spl(x_smooth)
# plot original data and spline line
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()

plt.show()
```

<img width="707" height="492" alt="image" src="https://github.com/user-attachments/assets/4956227d-7609-44cb-97f9-882a2ef23f1b" />



```
import matplotlib.pyplot as plt
# heights of bars
height = [10, 24, 36, 40, 5]
#labels for bars
names = ['one', 'two', 'three', 'four', 'five']
# plotting a bar chart
c1=['red', 'green']
c2=['b', 'g'] # we can use this for color
plt.bar (names, height, width=0.8, color=c1)
#naming the x-axis
plt.xlabel('x axis')
#naming the y-axis
plt.ylabel('y axis') 
# plot title
plt.title('My bar chart!')
#function to show the plot
plt.show()
```

<img width="772" height="535" alt="image" src="https://github.com/user-attachments/assets/e2398795-1da1-487d-851c-f32858680977" />



```
import matplotlib.pyplot as plt
# frequencies
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
# setting the ranges and no. of intervals
range = (0, 100)
bins=10
# plotting a histogram
plt.hist(ages, bins, range, color='green', histtype='bar', rwidth=0.8)
# x-axis label
plt.xlabel('age')
# frequency label
plt.ylabel('No. of people')
# plot title
plt.title('My histogram')
# function to show the plot
plt.show()
```


<img width="795" height="583" alt="image" src="https://github.com/user-attachments/assets/ed1335bb-750a-40a1-9b84-e16a749d1d0e" />



```
import matplotlib.pyplot as plt
#generate fake data
x = [2, 1, 6, 4, 2, 4, 8, 9, 4, 2, 4, 10, 6, 4, 5, 7, 7, 3, 2, 7, 5, 3, 5, 2, 1]
#plot for a histogram
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```


<img width="680" height="507" alt="image" src="https://github.com/user-attachments/assets/180ad0c9-b2cc-40a0-a60a-c3034a0e541d" />


```
np.random.seed (0)
data = np.random.normal(loc=0, scale=1, size=100)
data
```


<img width="717" height="401" alt="image" src="https://github.com/user-attachments/assets/ad5d3b39-b8fe-4ef1-96f2-c7ab26426c71" />


```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
 ```


<img width="700" height="552" alt="image" src="https://github.com/user-attachments/assets/65eeb052-3f85-4dce-8927-e2cb812a5453" />



```
import matplotlib.pyplot as plt
# defining labels
activities = ['eat', 'sleep', 'work', 'play']
# portion covered by each label
slices = [3, 7, 8, 6]
# color for each label
colors = ['r', 'y', 'g', 'b']

plt.pie (slices, labels = activities, colors=colors,
startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1f%%')
# plotting legend
plt.legend()
# showing the plot
plt.show()
```

<img width="552" height="496" alt="image" src="https://github.com/user-attachments/assets/81c1e73c-fe23-4498-8662-edcabe183358" />



```
# Data to plot
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes <= [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)
# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```

<img width="657" height="472" alt="image" src="https://github.com/user-attachments/assets/c980ee1c-56e3-4e81-95a2-b5b144917a37" />


# Result:

 Thus, all the data visualization techniques of matplotlib has been implemented.
