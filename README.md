# dissolCases: Case files for dissolFoam snapshot dissol1706:

The cases were tested with OpenFOAM-v1706, together with the libraries and solvers from the following commits:
<br>dissolFoam      commit e8a926d 
<br>libsFoamAux     commit 23897c9
<br>dissolUtilties  commit 53b0557

The libraries and solvers should be arranged in the standard OpenFOAM manner under WM_PROJECT_USER_DIR/applications

There are three sets of cases:

1) dissolFrac - a simulation of a dissolving fracture, based on the experiments reported in Osselin et al. GRL 2016. The initial surface is created by Fourier synthesis followed by relaxation (with the dissolMotion solver).

2) dissolCirc - a simulation of a dissolving gypsum cylinder in the same microfluidic cell.

3) seededFracture - contains sample cases from a paper submitted to Water Resources Research in March 2018. Other cases can be easily created by editing the parameters D and lR in the file constant/transportProperties.  The remaining inputs are the same.

4) examples - contains sample outputs, including plots and movies as well as actual output files for a detailed comparison. Output files can be opened in Paraview when combined with the system and constant directories.

<br> dissolFrac (*.ogv): Movies of the concentration field and surface profile of a dissolving fracture
<br> dissolCirc (*.png): Renderings of concentration (C*.png) and images of the dissolving disk (S*.png) and contours (shapes.png) at every 10 time units (1 time unit is about 11 hours in real time).
<br> seededFracture (t*.png): Renderings of the fracture at different times, along with profiles across the width of the fracture (x) at z=250 and along the centerline (z).

The cases can be run by first executing the Mesh script, followed by Run np, where np is the number of processes; 16 or more cores are needed for a reasonably quick run. The script will run with any 1D or 2D decomposition (e.g. Run 8 2) or in serial mode (Run), although serial mode will be slow for these cases. The script will use the file hosts if it is present. For the dissolCirc case, the makeSTL script must be run before Mesh.

The simulations shown in examples were run with the following processor configurations:
<br>dissolFrac - Run 8 8    (np = 64)
<br>dissolCirc - Run 8 8    (np = 64)
<br>seededFrac - Run 16 1   (np = 16)
<br>To generate binary-identical data the same processor configurations must be used.
