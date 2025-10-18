A functionObject for remapping scalar fields at mesh nodes X to X + S, discrete times for t = mT.

It requires a displacement volVectorField S to exist in 0/.
The field S is expected to come from particle tracking simulations data x(X,T) = X - S(X,T). 

X + S likely does not sit on mesh nodes. This functionObject constructs a temporary scalar field C_new which is interpolated onto the mesh and replaces C before the map.
