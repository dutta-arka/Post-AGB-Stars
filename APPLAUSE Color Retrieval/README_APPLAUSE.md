## Description of The Code
This set of code does the following: For a given set of GAIA stars,
1. retrives the Plate ids and the source ids it matches with APPLAUSE DR4 and collectes them using it's source_xmatch  table.
2. Use the output from the last step and use source_calib table to get natural magnitude of the stars, along with color term (and error associated with them) and also crossmatch the GAIA IDs as error exists in the APPLAUSE archive while runing a TAP query to find from GAIA Id to source id. A crossmatch step helps remove those.
3. Finally we use all plate ids from different observatories and try to see if any plate with different emulsion (colr terms are atleast differn my 0.25) that are taken within 4 moths of each other contains the same object that we are interested in. If they do, then we use first order approximation of the magnitue calibration equation from Lacock et al. 2010 to find equivalent GAIA Bp and Rp values.


## Instructions to Run The Code
Combined files and individual files are uploaded in this google drive folder: https://drive.google.com/drive/folders/11U3avUIoD8SukXdUqJwNDFF9ZQ19ys6r?usp=sharing
