## Description of The Code
This set of code does the following: For a given set of GAIA stars,
1. Retrieves the plate IDs and the source IDs it matches with APPLAUSE DR4 and collects them using its source_xmatch  table.
2. Use the output from the last step and use the source_calib table to get the natural magnitude of the stars, along with the colour term (and the error associated with them) and also crossmatch the GAIA IDs as an error exists in the APPLAUSE archive while running a TAP query to find from GAIA Id to source id. A crossmatch step helps remove those.
3. Finally, we use all plate IDs from different observatories and try to see if any plate with different emulsions (colour terms are at least twice the combined error associated with both colour terms) that are taken within four months of each other contains the same object that we are interested. If they do, we use the first-order approximation of the magnitude calibration equation from Lacock et al. 2010 to find equivalent GAIA Bp and Rp values.

The .csv files can downloaded from the APPLAUSE archive.

## Instructions to Run The Code
Combined files and individual files are uploaded in this Google Drive folder: https://drive.google.com/drive/folders/11U3avUIoD8SukXdUqJwNDFF9ZQ19ys6r?usp=sharing
1. Download the existing .csv files given in this folder.
2. For this repository, we select a GAIA ID set from a catalogue of post-AGB stars (.csv file also attached). See https://doi.org/10.1093/mnrasl/slac088.
3. Open the Data_Retrieval.ipynb file and run the code (adjust the file's location). The notebook is self-explanatory.
