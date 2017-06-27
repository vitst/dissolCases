# dissolFoamTestCases
Test cases for dissolFoam solver.

seededFracture: commit acfa34a (develop)
    Dissolution of the flat fracture with small perturbation at the inlet
    Includes new flags for dissolMotion solver in pointMotionU
    scaleMotion   1.0;  -- scales the point displacement
    surfaceRlx    true; -- switches on/off relaxation on the patch
    edgeRlx       true; -- switches on/off relaxation on the edges 


* cylinder


* gypsumExperiment


dissolParaH: commit 711457d
    Dissolution of a parabola in a Hele-Shaw Cell - cfMesh grid
    Includes drag force from upper and lower walls
    
dissolCirc: commit 711457d
    Dissolution of a circle in a Hele-Shaw Cell - blockMesh grid
    Images show test of linearUpwind div scheme (left) vs upwind (right)
    Includes drag force from upper and lower walls

dissolCircCFM: commit 711457d
    Dissolution of a circle in a Hele-Shaw Cell - cfMesh grid
    Illustrates mesh instability with cfMesh generated grid (png)
    C.ogv shows blockMesh generated solution (left) vs cfMesh (right)
    Script to make stl files not nesessary - requires genBlockMeshDict scripts 


* triangle


