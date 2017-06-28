# dissolFoamTestCases: Test cases for dissolFoam solver

The commit levels are for dissolFoam and libsFoamAux respectively

seededFracture: commits acfa34a/1521d11 
    Dissolution of the flat fracture with small perturbation at the inlet
    Includes new flags for dissolMotion solver in pointMotionU
    scaleMotion   1.0;  -- scales the point displacement
    surfaceRlx    true; -- switches on/off relaxation on the patch
    edgeRlx       true; -- switches on/off relaxation on the edges 

dissolPara: commits 711457d/53f99f5
    Dissolution of a parabola in a Hele-Shaw Cell - cfMesh grid
    Includes drag force from upper and lower walls
    Mesh relaxation is very unstable - crashes at t=2
    
dissolCirc: commits 711457d/53f99f5
    Dissolution of a circle in a Hele-Shaw Cell - blockMesh grid
    Images show test of linearUpwind div scheme (left) vs upwind (right)
    Includes drag force from upper and lower walls

dissolCircCFM: commits 711457d/53f99f5
    Dissolution of a circle in a Hele-Shaw Cell - cfMesh grid
    Illustrates mesh instability with cfMesh generated grid (png)
    C.ogv shows blockMesh generated solution (left) vs cfMesh (right)
    Script to make stl files not nesessary - requires genBlockMeshDict scripts 


* cylinder


* gypsumExperiment


* triangle


