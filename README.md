# Utility of ctDNA in Non Small Cell Lung Cancer treated at the City of Hope

This repository presents the data and the analyses done for the manuscript "Utility of Circulating Tumor DNA in Identifying Somatic Mutations and Tracking Tumor Evolution in Patients with Non-small Cell Lung Cancer." `ctDNA.rda` R data has all the relevant datasets for the analysis.`ctDNA_NSCLC.Rmd`script has code for all the results described in the paper. 

# Datasets

You will need to load the `ctDNA.rda` for running the `ctDNA_NSCLC.Rmd` script:
prep_gg, prep_gone, prep_founddf, simp_concordance, alk_blood,alk_tissue,combo, multi.

1. prep_gg: This dataframe has 473 ctDNA samples from 370 unique NSCLC patients for ctDNA mutation analyses.
2. prep_gone: This dataframe has relevant clinical information regarding each of the 370 NSCLC patients for survival analyses
3. prep_founddf: This dataframe contains 64 matched samples and their relevant information for concordance analyses
4. simp_concordance: This is a simplified matrix indicating where gene level mutations were detected in the 64 matched ssamples.
5. alk_blood and alk_tissue: These dataframes presentss patient data who are positive for ALK-EML4 fusion in ctDNA and tissue matched samples
6. combo: This dataframe lists all the patient info - treatments and start date, tissue and ctDNA samples for tumor evolution analysis in patients G1, G8, G9, G59 and G220. 
7. multi: This dataframe has all the ctDNA information for patients with multiple ctDNA time points

**all dates are in relation to the first ctDNA sample collection date in each patients.

# Required R packages
1. ggplot2
2. survival
3. survmier
4. dplyr
5. ggplot2
6. gridExtra
7. ComplexHeatmap
8. GenVisR
9. stringr
10. discover