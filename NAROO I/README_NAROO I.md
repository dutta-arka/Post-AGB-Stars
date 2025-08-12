##A Work-In Progress?

Here, only the cross-matching of stars from the photographic plate to GAIA DR3 stars has been given. Considering:
1. Location in the sky by cross-matching and
2. Considering the proper motion of the stars,
 we can cross-match the given NAROO I plate details to the stars

Remember that after using SExtractor, zero points cannot be directly calculated; due to the nonlinearity of the photographic plate, one needs to do the colour calibration. However, a shortcut rough approximation could be done by selecting a short cone around the target stars. If a few of them are not variable and do not evolve rapidly, we can use them to calculate that star's photometric magnitude at that plate's natural photometric system.

 Here is one .ipynb file. This does two things
 1. Crossmatches all the stars with a given GAIA ID set.
 2. When given a plate, extract and crossmatch the sources.

Cone selection or even the entire plate colour calibration is possible to do for NAROO I, as there are not too many plates here. Those can be implemented, and once that is done, the methodology will be the same as for APPLAUSE code, except this will be faster as there will be no requirement for a query, and the data set will be smaller.
