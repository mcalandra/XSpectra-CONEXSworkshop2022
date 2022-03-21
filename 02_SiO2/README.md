# Si K-edge in SiO2

## How to execute this folder

Calculation of the spectrum in different planes

- <code>mpirun -np 4 pw.x -inp SiO2.scf.in > SiO2.scf.out</code>
- <code>../tools/upf2plotcore.sh ../pseudopotentials/Si_PBE_USPP.UPF > Si.wfc</code>
- <code>mpirun -np 4 xspectra.x -inp SiO2.xspectra_dip_plane.in > SiO2.xspectra_dip_plane.out</code>
- <code>mpirun -np 4 xspectra.x -inp SiO2.xspectra_dip_c.in > SiO2.xspectra_dip_c.out</code>

Examples of how simulation can be restarted

- <code>mpirun -np 4 xspectra.x -inp SiO2.xspectra_dip_restart_1.in > SiO2.xspectra_dip_restart_1.out</code>
- <code>mpirun -np 4 xspectra.x -inp SiO2.xspectra_dip_restart_2.in > SiO2.xspectra_dip_restart_2.out</code>
