# HomeWork


Simulation Parameters:

grid_size: Size of the 2D grid.
dx: Grid spacing.
dt: Time step.
duration: Total simulation time.
Initialization:

u, v: Arrays representing the x and y components of velocity, respectively.
h: Array representing the height of the water column.
Initial condition: A simple disturbance is introduced by setting a region in the center of the grid (h[40:60, 40:60]) to a height of 1.0.
Simulation Loop:

The simulation iterates over time steps from 0 to duration with a time step of dt.
In each iteration:
Gradients of velocity (du_dx, du_dy, dv_dx, dv_dy) and water height (dh_dx, dh_dy) are computed using NumPy's gradient function.
The shallow-water equations are then used to update the velocity (u and v) and water height (h) arrays. These equations are simplified for a 2D shallow-water system.
Visualization:

After the simulation is complete, the final state of the water height (h) is visualized using Matplotlib.
plt.imshow is used to create a 2D image plot of the water height with a blue colormap ('Blues').
plt.colorbar adds a colorbar to the plot, indicating the height values.
Title, labels, and axis extents are set for better understanding of the visualization.
plt.show() displays the final plot.
The simulation represents the evolution of a disturbance in the water column over time due to the application of the shallow-water equations. The visualization shows how the disturbance propagates and interacts with the surrounding environment.
