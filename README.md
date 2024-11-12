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
x1 = [1,2,3]
y1 = [2,4,1]
plt.plot(x1,y1,label="line 1")

x2=[1,2,3]
y2=[4,1,3]

plt.plot(x2,y2,label="line 2")

plt.xlabel("x - axis")
plt.ylabel("y - axis")
plt.title("Two lines on same graph!")
plt.legend()
plt.show()
```
![download](https://github.com/user-attachments/assets/2174e9d7-3e7b-4b64-8cf1-977abcd2d443)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',
linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel("x - axis")
plt.ylabel("y - axis")
plt.title('Some cool customizations!')
```
![download](https://github.com/user-attachments/assets/ce23b570-8cd3-4d5f-827d-ef08355f12f5)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![download](https://github.com/user-attachments/assets/147669e8-c4ff-40b5-af6d-c1ecc0826484)

```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
```
![download](https://github.com/user-attachments/assets/d522487e-bb7e-489b-8108-2368f94674a6)

```
years=range(2000,2012)
apples= [0.895,0.91,0.919,0.926,0.929,0.931,
0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,
0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```
![download](https://github.com/user-attachments/assets/25d8bdb2-6242-430a-8d38-0f3cbec7d81f)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/05f630f2-30bc-4f41-a9b7-0cacfc6def8c)

```
y
```
![image](https://github.com/user-attachments/assets/4a0dc9f6-ab18-42a2-b46a-afa2fe614460)

```
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![download](https://github.com/user-attachments/assets/c2a29451-537c-4924-b9b9-b18475b93375)

```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/8c7b6904-c16f-46b4-bba5-56130cb0bc6f)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![download](https://github.com/user-attachments/assets/ccf19cd2-723f-46bd-8c2f-bb32dff64299)

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
```
![download](https://github.com/user-attachments/assets/60a2b936-bf37-4479-a3d5-4bb410bccc76)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='orange')
plt.fill_between(x,y2,color='yellow')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![download](https://github.com/user-attachments/assets/ae26bea4-e1bd-40b2-a671-b86adbebaee0)

```
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.barh(names,values,color="yellowgreen")
plt.show()
```
![download](https://github.com/user-attachments/assets/154681e6-d48e-48e7-b8bb-8ce681ecc22f)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![download](https://github.com/user-attachments/assets/d75c4bfc-0766-4c7e-97a8-0882f912b79d)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,11]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![download](https://github.com/user-attachments/assets/d3a5851a-e982-4d50-ad4b-562cde67e7ac)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,
40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',
histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No.of people')
plt.title('My histogram')
plt.show()
```
![download](https://github.com/user-attachments/assets/6442a7b1-5009-436a-afe7-ccbadf1ad642)

```
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,
5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
```
![download](https://github.com/user-attachments/assets/893aaf17-6501-420f-92ce-e79e1da77387)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/5662c16f-f896-48e0-ad6f-cea0f702f12b)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box plot')
```
![download](https://github.com/user-attachments/assets/1688f195-92da-4bd3-8a7e-6c6a8a83cddb)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['purple','skyblue','pink','violet']
plt.pie(slices,labels=activities,colors=colors,startangle=90,
shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![download](https://github.com/user-attachments/assets/dcbd4cf9-7fa3-4a79-89bb-7fac9b515081)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,
autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![download](https://github.com/user-attachments/assets/36d3e142-62bb-4834-97ac-19e589eeea34)


# Result:
 
 Data Visualization using matplot python library for the given datas has been done.

