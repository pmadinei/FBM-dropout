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
    

<img width="862" alt="Screenshot 2023-03-21 at 9 27 27 PM" src="https://user-images.githubusercontent.com/45627032/226802189-353a62ab-d94f-4394-a221-a191d733f140.png">

<img width="862" alt="Screenshot 2023-03-21 at 9 28 11 PM" src="https://user-images.githubusercontent.com/45627032/226802297-04816a74-f86b-49f2-821a-3fb20694ab61.png">

<img width="862" alt="Screenshot 2023-03-21 at 9 28 27 PM" src="https://user-images.githubusercontent.com/45627032/226802370-ce829bbe-f68c-49b8-bf6e-c8eb617cc611.png">




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
