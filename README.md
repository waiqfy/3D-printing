# 3D-printing Slicer

Processing an STL file for 3D printing involves a crucial step known as slicing. STL files are designed to streamline slicing as a low-memory task by storing each triangle at a single location.

In this code, an ASCII .stl file is read and stored as a list of 3D points. These points are then projected onto a horizontal slicing plane. The projected 2D points are connected to form a list of segments, representing the trajectory of the 3D printer's extruder. Subsequently, there is a function that converts this trajectory into G-code, allowing direct interpretation by the 3D printer.
