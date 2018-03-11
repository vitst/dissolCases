# dissol1706: Case files for the snapshot dissol1706

The case files run two samples of the cases reported in a paper submitted to
Water Resources Research in March 2018. Other cases can be easily created
by editing the parameters D and lR in the file constant/transportProperties.
The remaining inputs are the same.

The cases can be run by first executing the Mesh script, followed by
Run np, where np is the number of processes; 16 cores are needed
for a quick (12 hour) run. The script will run with any 1D or 2D
decomposition (e.g. Run 8 2) or in serial mode (Run), although serial mode
will be slow for these cases. The script will use the file hosts if it is
present.

The cases require a recent version of OpenFOAM, together with the libraries
and solvers from the dissol1706 snapshot. The codes were tested with
OpenFOAM-v1706. Some sample outputs are in the subdirectory examples.
It is too large for the snapshot submitted to WRR but can be found at
https://github.com/vitst/dissolFoamCases/tree/master/dissol1706/examples.

