# NOMP
N-Body OpenMP

This is a simple NBody simulation using Verlet-Algorithm. The interaction between particles is LennardJones. The are two versions, and one utilizes OpenMP to parallelize the code with OpenMP over 8 (or else) threads. It's just used for the bulky part of the algorithm which is updating the particles fields. I dunno why I didnt also do it for the next loop which updates _pos_ with _npos_.

The parameters are set using _#define_. _n_ is number of particles, _T_ is number of timesteps to sim, _dt_ is the delta-time of each timestep, _Rm_ and _E_ are the parameters of the LJ potential. I think you can make the heads of tails of the code, no twist really.

Dont forget _-fopenmp_ option when compiling the omp code. 
