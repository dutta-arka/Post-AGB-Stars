MESA MIST tracks are available for anyone to download here: https://waps.cfa.harvard.edu/MIST/index.html.

## Basics of MIST Tracks
MIST tracks are of two types:
1. Isochrones tracks of identical mass.
3. Evolutionary tracks of the same star.

These tracks can be downloaded in bulk or more customised from https://waps.cfa.harvard.edu/MIST/interp_tracks.html. For our study, we used .eep.cmd type tracks. The basic code is in Fortran. However, the tracks can be opened using Python (see https://github.com/jieunchoi/MIST_codes.git).

A crude idea of how to handle and tweak these codes is in the MIST.ipynb file.
1. There are codes for opening the files and accessing the columns.
2. How to plot multiple tracks and overlay them.
3. The fastest region for data selection could be selected from GAIA.
