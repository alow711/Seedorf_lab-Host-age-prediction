# host-age-prediction
**This repository contains Qiime2 codes and outputs used for "Host-age prediction from fecal microbiota composition in male C57BL/6J mice"**

Authors:Adrian Low, Melissa Soh, Sou Miyake and Henning Seedorf

**“Qiime2_code_metadata” folder:**

•	Qiime2-code.txt- codes for Qiime2 2 v.2021.4, indicating the input, output, and metadata used.

•	manifest-all- lists the fastq files that were analyzed.
Refer to https://docs.qiime2.org/ for description of headings

•	metadata.txt- contains samples for longitudinal study (starts with a numeral e.g. 5.F10_11118_53) and samples for dietary study (starts with M e.g. M13-26-Jun). N=433 for longitudinal study; N=406 for dietary study.

"#SampleID" (Sample identity), "PrimerSequence" (515F primer sequence), "Sampling-date" (date of fecal sampling in Month/Day/Year), "Timeline_diet" (dietary study timeline in days), "Age_wk" (Age of mice in weeks), "Life_phase" (Life phase category for longitudinal study), "mouse" (mouse identity number for longitudinal study), "Cage" (cage number for longitudinal study), "Cage_category" (cage number spelt in words)
•	LTS-metadata.csv- contains samples for longitudinal study only.

Additional headings “Age_weeks” (categorical age of mice in weeks), “Timeline_LTS” (experimental timeline in days), “stages” (life phase or life stage).
"#SampleID" (Sample identity), "PrimerSequence" (515F primer sequence), "Age(days)" (Mice age in days), "Age_wk" (Age of mice in weeks), "Timeline_LTS" (longitudinal study timeline in days), "stages" (Life phase category for longitudinal study).

•	LTS-metadata_cage.csv
As of above including “Diet” (diet type SD standard diet or WD Western diet for dietary study), “stages2” (includes intermediate life stages), Year (Year 1 or Year 2 time points).

•	biogeo_30percent_unknown.txt- A list to filter the dietary study samples to exclude samples with more than 30% unknown from sourcetracker analysis. This is used to filter the rep-seq and table so that a custom PCoA plot (Figure 5C) which matched the SourceTracker data in Figure 5B.

•	biogeo-samples_Dec21.csv- a metadata used to Group the samples “GroupID”

•	biogeo-merged_Dec21.csv-a metadata used for creating the custom PCoA emperor plot (Figure 5C).

**“Qiime2_denoising" folder:** contains denoising, tables, rep-seqs of combined longitudinal and dietary study data. 
"single-end-trim-demux.qza" is not provided due to its large file size

**"Qiime2_Longitudinal_study"** contains all *qza and *qzv files specific to longitudinal study.

**"Qiime2_Longitudinal_study2"** contains output folders for core-metrics and feature-volatility (Random forest ASV prediction) for longitudinal study.

**"Qiime2_Dietary_study"** contains output for dietary study.

**"Sourcetracker" folder:** contains 2 subfolders for SourceTacker v.0.9.1 https://github.com/danknights/sourcetracker
•	Longitudinal - Longitudinal study samples only 5 time points as "source". Figure 4 of manuscript

•	Longitudinal+Dietary - same configuration as Longitudinal including 5 time points of control mice from Dietary study. Refer to Figure 5 of the manuscript.
  Each subfolder contains
  
  - otus.txt - tab delimited file of ASV table (not rarefied)
  
  - map.txt - mapping file
Sample IDs with _ were replaced with -
