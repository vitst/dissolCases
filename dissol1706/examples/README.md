# dissol1706: Examples from dissol1706

Data was generated from case files Pe20lR1 and Pe80lR1.
The directories contain snapshots from Paraview and sample output files.

The output files serve as a check for future runs. They can be viewed
in Paraview when combined with the system and constant directories.
The png files show renderings of the fracture at different times, along
with profiles (C and U_Z) taken across the width of the fracture (x)
at z=250 and along the centerline (z). Note that the coordinate system
in the code (z = flow, x = width, y = aperture) is rotated from the one
in the paper (x = flow, y = width, z = aperture).

The directories Upw1 and Upw2 refer to first-order and second-order upwind
differencing of the convective flux. In the paper we used the first-order
but it is more dispersive than the second-order scheme. The case files
(in the directory above) are set up to use the second-order scheme. The
examples indicate the small but noticeable differences.
