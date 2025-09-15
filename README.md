# Generating an animation file for Visual Molecular Dynamics (VMD) software in Fortran
![image alt](https://github.com/atomicadi/Animate-a-rotating-molecule-on-solid-surface_in-Fortran/blob/77e654e17ab198b5ca6d11fa38d2ae6e7e3bff33/Untitled.001.png)
Visual Molecular Dynamics (VMD) is a widely used molecular visualization and analysis program in the fields of computational chemistry and biology. VMD typically reads the coordinates of each step in a simulation (e.g., molecular dynamics, optimization, etc.) from a single file (commonly in .xyz format) and visualizes the system as an animation.

In this case, a molecule on a solid surface is rotated (Example 1) and translated (Example 2). After each rotation or translation, a separate coordinate file (.xyz format) is generated corresponding to that specific perturbation.


Once the total number of coordinate files has been specified, the Fortran code (**animation_rotation.f90**) runs a loop to sequentially open, read, and store each perturbed coordinate file into a single animation file named **animation_rotation.xyz**. This combined file can then be loaded into VMD to animate the structural changes of the system on screen.
