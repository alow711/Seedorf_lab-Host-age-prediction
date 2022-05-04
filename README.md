# host-age-prediction
This repository contains scripts and data files used for "Host-age prediction from fecal microbiota composition in male C57BL/6J mice"

Authors:Adrian Low, Melissa Soh, Sou Miyake and Henning Seedorf

Here are brief descriptions of each folder:

Qiime2_code_metadata:

metadata.txt- contains samples for longitudinal study (starts with a numeral e.g. 5.F10_11118_53) and samples for dietary study (starts with M e.g. M13-26-Jun).
Columns "#SampleID" (Sample identity), "PrimerSequence" (515F primer sequence), "Diet" (SD-standard diet, WD-western diet; used to differentiate dietary treatment), "Timeline_diet" (dietary study timeline in days), "Age_wk" (Age of mice in weeks), "Life_phase" (Life phase category for longitudinal study), "mouse" (mouse identity number), "Cage" (cage number), "Cage_category" (cage number spelt in words)
N=433 for longitudinal study;
N=406 for dietary study.

LTS-metadata.csv- contains samples for longitudinal study only.
"#SampleID" (Sample identity), "PrimerSequence" (515F primer sequence), "Age(days)" (Mice age in days), "Age_wk" (Age of mice in weeks), "Timeline_LTS" (longitudinal study timeline in days), "stages" (Life phase category for longitudinal study).


Qiime2-code.txt- codes for Qiime2

Qiime2_output
Qiime2 *.qza, *.qzv files.
"single-end-trim-demux.qza" is not provided due to its large file size

Qiime2_code_metadata:contains metadata and codes used with QIIME 2 v.2021.4

Qiime2_data_files:contains the QIIME output

Folder: Sourcetracker contains 2 subfolders

Longitudinal - Longitudinal study samples only 5 time points as "source". Figure 4 of manuscript

Longitudinal+Dietary - same configuration as Longitudinal. Dietary study includes 5 time points as "source". Figure 5 of manuscript.
  Each subfolder contains
    otus.txt - tab delimited file of ASV table (not rarefied)
    map.txt - mapping file
*Replaced _ with - for R.
