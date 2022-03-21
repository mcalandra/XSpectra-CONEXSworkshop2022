# Cu L-Edges with fractional core hole

## How to execute this folder

Prepare the core wavefunctions

- <code>../tools/upf2plotcore.sh ../pseudopotentials/Cu_US_PBE_3pj_lowE.UPF > Cu.wfc</code>

XANES spectrum without core hole

- <code>mpirun -np 4 pw.x -inp Cu.scf.in > Cu.scf.out</code>
- <code>mpirun -np 4 xspectra.x -inp Cu_xspectra.in > Cu_xspectra.out</code>

2<em>p</em> to <em>d</em> transitions only!

- <code>mpirun -np 4 xspectra.x -inp Cu_xspectra_lplus.in > Cu_xspectra_lplus.out</code>

XANES spectrum with half a core hole

- <code>mpirun -np 4 pw.x -inp Cu_halfh.scf.in > Cu_halfh.scf.out</code>
- <code>mpirun -np 4 xspectra.x -inp Cu_halfh_xspectra.in > Cu_halfh_xspectra.out</code>
- <code>mpirun -np 4 xspectra.x -inp Cu_halfh_xspectra_replot.in > Cu_halfh_xspectra_replot.out</code>
