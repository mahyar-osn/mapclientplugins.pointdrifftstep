# mapclientplugins.parametricfittingstep
MAP Client plugin for performing rigid and non-rigid fitting of a scaffold to image data 

This plugin works as a stand-alone module to fit two sets of data.
The current version (0.1.0) was built to satisfy the requirements to fit a 3D, tricubic hermite heart FE model to 2D image of heart. 

# Requirements: 
- Numpy
- MAPClient ()
- mapclientplugins.meshgeneratorstep () - This is temporary.

# Fiducial landmarks: 
The 0.1.0 version requires 11 manually placed fiducial points on the image data - see 'fiducial_landmarks_example.png'.

# Configs:
For convenience, a config directory is also added. Put this into your workflow directory in order to load the image and mesh data
in a nice orientation.

# Fitting: 
Once the fiducial landmarks are placed on the image data, run 'Rigid Fitting' so that the mesh is scaled, rotated, and trnaslated, 
then run 'Non-Rigid Fitting' to deform the mesh with respect to the heart image data.
