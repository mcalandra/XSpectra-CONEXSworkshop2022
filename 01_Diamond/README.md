# C K-Edge in Diamond

## How to execute this folder

Diamond example with no core-hole

- <code>mpirun -np 4 pw.x -inp diamond.scf.in > diamond.scf.out</code>
- <code>mpirun -np 4 xspectra.x -inp diamond.xspectra.in > diamond.xspectra.out</code>
- <code>mpirun -np 4 xspectra.x -inp diamond.xspectra_replot.in > diamond.xspectra_replot.out</code>

Diamond example with hole in 1<em>s</em>

- <code>mpirun -np 4 pw.x -inp diamondh.scf.in > diamondh.scf.out</code>
- <code>mpirun -np 4 xspectra.x -inp diamondh.xspectra.in > diamondh.xspectra.out</code>


