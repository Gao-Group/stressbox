# stressbox
Two scripts in this repository: stressbox.py and opt_example.py are used to apply stress (including PK stress and Cauchy stress) in molecular statics simulations.
The method is reported in the following paper:
Arman Ghasemi, Wei Gao. "A method to apply Piola-Kirchhoff stress in molecular statics simulations", submitted. 

To use the code:
1. Download Atomic Simulation Environment (ASE) package from https://wiki.fysik.dtu.dk/ase/, 3.19.0 version was used to test the scripts.
2. Copy stressbox.py to ase-3.19.0/ase/ folder.
3. Add ASE directory to your $PYTHONPATH
4. Set the lammps environmental variable in your system: export ASE_LAMMPSRUN_COMMAND="mpirun -np 2 lmp_mpi", where lmp_mpi is the compiled mpi version of lammps 
5. To run the example: copy opt_example.py along with two lammps data files and SW potential file into your working directory.
6. Run the code: python3 opt_example.py.
