# Pluripotency analysis
This script quantifies the percentage of cells in 2D images that co-express two pluripotency markers. The inputs are i) a representative single-channel image of nuclei, ii) representative single-channel images of isotype control staining for each pluripotency marker, and iii) an input folder path containing multi-channel images of nuclei and pluripotency markers. The output is a file containing and the percentage of cells that co-express markers. The pipeline is comprised of the following steps:
1. Measure the average somata size. Users will need to provide a .tif image of a nuclei marker, and use the elliptical/oval tool to estimate the size of a single somata.
 
2. Establish a lower threshold value for pluripotency mask generation. The user will need to provide matched isotype control .tif images for each pluripotency marker, and set the upper threshold for background fluorescence intensity so that it may be subtracted from images throughout processing.

3. Select input folder containing .czi images that include all channels. Select output folder where metrics will be saved as a .csv file.
