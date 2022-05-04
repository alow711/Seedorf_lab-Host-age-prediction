# host-age-prediction
This repository contains scripts and data files used for "Host-age prediction from fecal microbiota composition in male C57BL/6J mice"

Authors:Adrian Low, Melissa Soh, Sou Miyake and Henning Seedorf

Here are brief descriptions of each folder:

metadata.tsv- contains samples for longitudinal study (starts with a numeral e.g. 5.F10_11118_53) and samples for dietary study (starts with M e.g. M13-26-Jun).
N=433 for longitudinal study
N=406 for dietary study

Qiime2_code_metadata:contains metadata and codes used with QIIME 2 v.2021.4

Qiime2_data_files:contains the QIIME output

Folder: Sourcetracker contains 2 subfolders

Longitudinal - Longitudinal study samples only 5 time points as "source". Figure 4 of manuscript

Longitudinal+Dietary - same configuration as Longitudinal. Dietary study includes 5 time points as "source". Figure 5 of manuscript.
  Each subfolder contains
    otus.txt - tab delimited file of ASV table (not rarefied)
    map.txt - mapping file
*Replaced _ with - for R.
