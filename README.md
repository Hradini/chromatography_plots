# Chromatic Separation Curves

This repository contains 
- jupyter notebooks 
	- to clean up .txt output files from size-exclusion chromatography runs and produce .csv files.
	- to generate chromatic separation curves, $K_{av}$ values and estimate molecular weight of samples.
- Raw_data/ contains sample input and output files for the converting notebook.

### ConvertingRawToCsv.ipynb
<b> Input </b> : 
- txt file saved as .csv. (open txt file in excel and save as .csv)
- Input and output paths

<b> Output </b> : 
- .csv file that has 2 columns, Volume and Abs. With only the values after injection ( positive values of the elution volume)

<b> Libraries needed: </b>
- pandas
- matplotlib
- os

### Chromatography_plots.ipynb
<b> Input </b> : 
- .csv file with elution volume and absorbance information for sample.
- .csv file with elution volume and absorbance information for markers OR information about the markers that can be manually entered.

<b> Output </b> : 
- Chromatographic separation curves
	- Absorbance vs. Elution Volume for markers with molecular weight markings.
	- Absorbance vs. Elution Volume for sample protein with molecular weight markings.
- $K_{av}$ values

<b> Libraries needed: </b>
- pandas
- matplotlib
- numpy
- scipy
- math
- sklearn

### References

- [3.4.2. Gel Exclusion Chromatography](https://chem.libretexts.org/@go/page/165276).  

- [Using a Gel Filtration Chromatogram to Estimate Molecular Weight](https://bitesizebio.com/29685/determine-molecular-weight-gel-filtration-chromatogram/)

- [Size Exclusion Chromatography Handbook ](https://www.cytivalifesciences.com/en/us/support/handbooks)
