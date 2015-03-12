# tmaps
Time machine automated python scripts for generating interactive zoomable videos for sharing transient AD Hydro model output.

This script was developed in the linux environment.

Ruby needs to be installed so that the time machine portion of the script can run.

In order to run the python script tmaps0.0.1.py, the user needs to have the tmc-1.1.0-linux folder and it's contents located in the same directory as the script. This folder contains all the ruby scripts that will process and generate the time machine visualizer.

There are two netcdf files that are expected to be located in the same local directory as the script - they are the geometery.nc and the display.nc files. Both of these files are generated for/from the AD Hydro program.

Finaly, there is a post processing code that is ran on the AD Hydro output that generates .xmf files so that the paraview module in python can parse the netcdf files correctly for rendering. Please make sure the mesh_display.xmf file is in the same directory as tmaps0.0.1.py.

For changing parameters to be rendered, contuor themes, and opacity, the user will adjust these at the beginning of the script portion after the methods and classes have been delcared on line 1150.

The numbe of cores that will be used in the time machine portion can be adjusted on line 1216

