# VHS-1256-b-JWST-spectral-extraction

Download JWST data for VHS1256 b from MAST (https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html) 
In the main MAST site, click "Advanced Search".
Then select JWST among missions, then select only NIRSpec and MIRI among instruments. Then, provide the object name (Use a SIMBAD-recognizable name: SIPS J1256-1257)
There should be ~25 data sets available to download.

From STScI JWST Data Analysis Toolbox page, click on Data Analysis Notebooks
(https://www.stsci.edu/jwst/science-execution/data-analysis-toolbox)
Find appropriate tutorials (MIRI → MRS Cube Analysis, NIRSpec → IFU Optimal Spectral Extraction)

Notes:
- For NIRSpec: The tutorial suggests to use a PSF model for an optimal extraction, but I could not find a WebbPSF that fit our data, so non-optimal extraction was used.
- For MIRI: I was not sure how to handle the different channels for each mode. Also, I was unable to find the target for extraction, as the data was too noisy.
