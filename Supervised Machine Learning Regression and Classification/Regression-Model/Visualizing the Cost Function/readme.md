# Visualizing the Cost Function

<br>
<br>

<div align="center">
  
![](https://github.com/dystaSatria/Machine-Learning/blob/main/Supervised%20Machine%20Learning%20Regression%20and%20Classification/Regression-Model/Visualizing%20the%20Cost%20Function/Screenshot%20(968).png)

![](https://github.com/dystaSatria/Machine-Learning/blob/main/Supervised%20Machine%20Learning%20Regression%20and%20Classification/Regression-Model/Visualizing%20the%20Cost%20Function/Screenshot%20(969).png)

</div>

Example : 


```py
import matplotlib.pyplot as plt
import numpy as np

from matplotlib import cm
from matplotlib.ticker import LinearLocator

fig, ax = plt.subplots(subplot_kw={"projection": "3d"})

# Make data.
X = np.arange(-5, 5, 0.25)
Y = np.arange(-5, 5, 0.25)
X, Y = np.meshgrid(X, Y)
R = np.sqrt(X**2 + Y**2)
Z = np.sin(R)

# Plot the surface.
surf = ax.plot_surface(X, Y, Z, cmap=cm.coolwarm,
                       linewidth=0, antialiased=False)

# Customize the z axis.
ax.set_zlim(-1.01, 1.01)
ax.zaxis.set_major_locator(LinearLocator(10))
# A StrMethodFormatter is used automatically
ax.zaxis.set_major_formatter('{x:.02f}')

# Add a color bar which maps values to colors.
fig.colorbar(surf, shrink=0.5, aspect=5)

plt.show()
```

<br><br>

<div align="center">
  
![](https://github.com/dystaSatria/Machine-Learning/blob/main/Supervised%20Machine%20Learning%20Regression%20and%20Classification/Regression-Model/Visualizing%20the%20Cost%20Function/Screenshot%20(970).png)

![](https://github.com/dystaSatria/Machine-Learning/blob/main/Supervised%20Machine%20Learning%20Regression%20and%20Classification/Regression-Model/Visualizing%20the%20Cost%20Function/Screenshot%20(971).png)

![](https://github.com/dystaSatria/Machine-Learning/blob/main/Supervised%20Machine%20Learning%20Regression%20and%20Classification/Regression-Model/Visualizing%20the%20Cost%20Function/Screenshot%20(970).png)

</div>


## Option Code Lab 

### Check the C1_W1_Lab03_Cost_function_Soln.ipynb

### Installation

- Download the sources like:
  - C1_W1_Lab03_Cost_function_Soln.ipynb
  - lab_utils_common.py
  - lab_utils_uni.py
 
- Open Google Collabs
- Import the downloaded source


