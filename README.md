# A highly customizable Fractional Brownian Motion Dropout algorithm inspired by brain's serotonergic system

This algorithm simulates Fractional Brownian Motion (FBM) agents on a rectangular plane with equal
relative spacing between squares. The class determines the size of the squares based on
    the values of 'plane_size', 'grid_shape', and 'neuron_spacing'. It also adds a border
    around the rectangle plane with a width of square edge / 2. The class generates 'n_fibers'
    number of random coordinates in the rectangle and simulates an FBM agent from each
    coordinate with a Hurst exponent of 'hurst'. The time of each FBM path is set to 'T'.
    The class uses standard FBM (σ = 1) and sets the time-distance between two consecutive
    points in FBM paths to 'deltaT'. The length of the moving fiber, in points, is set to
    'fiber_length' and the speed (offset) of fibers in each iteration, in points, is set to
    'fiber_speed'. The factor that translates the FBM-path coordinates to the rectangle
    coordinates (fbmToRec) is also set.
    
![image](https://user-images.githubusercontent.com/45627032/226737121-d8a5b18b-1e5b-4c5e-ae40-d3b692db3920.png) ![image](https://user-images.githubusercontent.com/45627032/226737910-446cd064-e4a0-42ab-ade9-0dfcb15bebd4.png) ![image](https://user-images.githubusercontent.com/45627032/226738439-bf7eb846-abd0-4c32-9eff-6d578eeb431e.png)





### Hyperparameters to play with:
plane_size (tuple): Tuple of two integers representing the size of the plane in X and Y dimensions.

grid_shape (tuple): Tuple of two integers representing the number of rows and columns in the rectangular grid.

spacing (float): Float representing the spacing between neurons.

hurst (float): Float representing the Hurst parameter used in the FBM agent.

n_fibers (int): Integer representing the number of FBM agents.

fiber_length (int): Integer representing the number of points in each FBM agent.

T (float): Float representing the time parameter for the FBM agent.

deltaT (float): Float representing the time step for the FBM agent. Default value is None.

fiber_speed (int): Integer >=1 representing the speed of the FBM agent. Default value is 1.

max_iters: (int): Integer representing the maximum number of forward calls during each epoch. Default value is 1000.

fiber_size: (float): Float representing the width of the fibers for visualization. Default value is 1.5.


Good luck!
