Vector Field Manifold Visualization
===================================

This project contains the files necessary to compute the stable or unstable manifold of a vector field using matlab, and then create a vtk file to be read by paraview for visualization. Specifically, we consider the system du/dt=F(u(t)), where u(t)=(x(t),y(t),z(t)) with a fixed point where F(fixed point) = 0. In the case of a stable manifold, we find the set of points such that as t->infinity, u(t) -> the fixed point. In the case of the unstable manifold, we find the set of points such that as t->negative_infinity, u(t) -> the fixed point.

Instructions
------------

- Download the files for this program from github. If you are not familiar with how to pull a github repo, simply click the "Download Zip" button on the right side of the github page and extract the files into a folder on your local machine.
- Edit the file myVectorField.m. It contains several examples in the comments. Only 1 example should be uncommented. You can also create your own vector field using the same style as shown in that file.
- (Optional) Open options.m and change any of the configuration options. This includes which method is used to calculate the manifold, how often the scheme adapts (interpolates new points), and how many time steps are saved in the output. 
- Run the matlab file main.m.
- Download and install paraview. Open the manifold.vtk file that was created when you ran main.m.