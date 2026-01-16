# Scatter-Plots-BoxPlots-in-Python

a. Python BoxPlot

import matplotlib.pyplot as plt

import numpy as np

np.random.seed(12)

one=np.random.normal(150,15,250)

two=np.random.normal(90,40,210)

three=np.random.normal(100,40,210)

four=np.random.normal(90,50,210)

to_plot=[one,two,three,four]

fig=plt.figure(1,figsize=(9,6))

ax=fig.add_subplot(111)

bp=ax.boxplot(to_plot)

fig.savefig('boxplot.png',bbox_inches='tight')

plt.show()

<img width="900" height="600" alt="boxplot matplotlib" src="https://github.com/user-attachments/assets/73042887-4d2c-4488-82be-6b0aeb5fc50f" />

b. Python Scatter Plot using plt.plot

np.random.seed(1867543)

N=50

x=y=colors=np.random.rand(N)

area = (30 * np.random.rand(N))**2

plt.scatter(x,y, s=area, c=colors, alpha=0.5)

<matplotlib.collections.PathCollection object at 0x0000027C49D23E00>

plt.show()

<img width="640" height="480" alt="seed(1867543)" src="https://github.com/user-attachments/assets/a15c3792-c345-407f-a931-f74bc1b5acf7" />

import math

x=np.linspace(0,20,40)

y=np.sin(x)

plt.plot(x,y,'o',color='purple')

plt.show()

<img width="640" height="480" alt="using plt plot" src="https://github.com/user-attachments/assets/51a7affa-3183-4fbf-b628-661ac4c0914d" />

plt.plot(x,y,'-ok')

plt.show()

<img width="640" height="480" alt="using plt plot png2" src="https://github.com/user-attachments/assets/553cc4a3-df40-4e4f-b0de-b2ec32c530d5" />


plt.plot(x,y,'-p',color='orange',

     markersize=15,linewidth=4,
     markerfacecolor='white',
     markeredgecolor='black',
     markeredgewidth=1)
     
plt.show()

<img width="640" height="480" alt="using plt plot png3" src="https://github.com/user-attachments/assets/450c2e21-e232-40ad-af61-a37bdf657053" />

c. More than one plot

plt.plot(np.random.rand(10),'*')

plt.plot(np.random.rand(5),'o')

plt.show()

<img width="640" height="480" alt="more than one plot" src="https://github.com/user-attachments/assets/648477b8-b570-4489-8a01-51dc4431077d" />

