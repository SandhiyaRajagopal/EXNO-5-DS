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
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
```
![image](https://github.com/user-attachments/assets/259636ff-7f00-45af-9be0-9b99b473ea04)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
```
![image](https://github.com/user-attachments/assets/93217a90-7c95-4670-b18c-24f91c6dd90a)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.92,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.xlabel('Year')
plt.ylabel('Yield')
plt.plot(years,apples,label='Apples')
plt.plot(years,oranges,label='Oranges')
plt.legend()
```
![image](https://github.com/user-attachments/assets/2cf53ebf-6f10-4bcd-b795-93330960f688)
```
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
```
![image](https://github.com/user-attachments/assets/ab78fc46-a50d-4767-828c-0ef21a43dc04)
```
x_values=[1,2,3,4,5,6,7,8,9,10]
y_values=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x_values,y_values,label="square" ,s=30,color="blue",marker="*")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("My scatter plot")
plt.legend()
```
![image](https://github.com/user-attachments/assets/294a1318-7797-4a34-8a3a-084e598c649e)
```
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
print(x)
print(y)
```
![image](https://github.com/user-attachments/assets/9233bbd7-cbdd-4411-944f-5bfc05a59b1a)
```
plt.scatter(x,y,c='b')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Graph in 2D')
plt.savefig('scatter.jpeg')
```
![image](https://github.com/user-attachments/assets/ccfb97cd-118b-47ec-aa30-61cbcf2e5de2)
```
x=np.arange(0,10)
y=x*x
y
```
![image](https://github.com/user-attachments/assets/9b24582d-3049-4178-b2bb-afb7c99a6b5e)
```
plt.plot(x,y,'r*',linestyle='dashed',linewidth=5,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D diagram')
```
![image](https://github.com/user-attachments/assets/5dbda4d4-7828-4c0b-b642-a9f54e0fc59f)
```
np.pi
```
![image](https://github.com/user-attachments/assets/14fc000e-1e32-48b2-9751-fef39307cf73)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title('Sine wave')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.plot(x,y)
```
![image](https://github.com/user-attachments/assets/df16b6ce-4f27-4945-bd48-581fae54a759)
```
plt.subplot(2,2,1)
plt.plot(x,y,'b--')
plt.subplot(2,2,2)
plt.plot(x,y,'r*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![image](https://github.com/user-attachments/assets/06077afb-48c3-4876-99c2-9e2a24de2e6d)
```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='grey')
plt.fill_between(x,y2,color='lightcoral')
plt.plot(x,y1,color='green')
plt.plot(x,y2,color='yellow')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/a671ebab-30c5-4d9e-9d27-ed02e8b06e9f)
```
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2','Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/d0149017-ac8b-4e89-92ab-c355cd0f5f06)
```
val=[5,6,3,7,2]
name=["A","B","C","D","E"]
plt.bar(name,val,color='pink')
plt.show()
```
![image](https://github.com/user-attachments/assets/518cafcf-88ef-486e-9ae5-5dc2f8297710)
```
h=[10,24,36,40,100]
name=['one','two','three','four','five']
c1=['r','g']
c2=['b','y']
plt.bar(name,h,color=c1,width=0.5)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Bar graph')
plt.show()
```
![image](https://github.com/user-attachments/assets/e2dfab59-9d41-4b2d-90fb-270056cf0a03)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='yellow')
plt.bar(x2,y2,color='pink')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Bar graph')
plt.show()
```
![image](https://github.com/user-attachments/assets/d1bf43c7-ffe0-4911-a5b5-7db81f93a84e)

# Result:
 Include your result here
