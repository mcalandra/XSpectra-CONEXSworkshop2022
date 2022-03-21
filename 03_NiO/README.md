# Ni K-edge in NiO

## How to execute this folder

XANES spectrum in the dipole approximation

- <code>mpirun -np 4 pw.x -inp NiO.scf.in > NiO.scf.out</code>
- <code>../tools/upf2plotcore.sh ../pseudopotentials/Ni_PBE_TM_2pj.UPF > Ni.wfc</code>
- <code>mpirun -np 4 xspectra.x -inp NiO.xspectra_dip.in > NiO.xspectra_dip.out</code>
- <code>mpirun -np 4 xspectra.x -inp NiO.xspectra_dip_replot.in > NiO.xspectra_dip_replot.out</code>

XANES spectrum in the quadrupole approximation

- <code>mpirun -np 4 xspectra.x -inp NiO.xspectra_qua.in > NiO.xspectra_qua.out</code>
