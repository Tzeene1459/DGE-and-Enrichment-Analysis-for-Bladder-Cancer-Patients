
# Phase III – Immuno-Oncology Analysis of Tumor Infiltrating Immune Cells with CiberSort

## Objectives: 

Exploring changes in bladder tumor microenvironment at different stages of cancer and comparing it with the immunological microenvironment in baseline bladder tissue sample. 

This analysis was conducted on stage 2 bladder cancer tissue in comparison to stage 1, and stage 1 bladder cancer tissue in comparison to precancerous stage. 

## Steps Performed in this Analysis: 

1.	I uploaded the input files to Cibersort keeping the LM22.txt file as signature, and the remaining three input files (Precancerous, Stage 1 and Stage 2) as mixture type files. 
 
2.	I ran the cibersort analysis with the configuration Impute Cell Fractions for Analysis Module. Selected the Custom analysis mode to custom input the lm22.txt as signature matrix file,  and one of the aforementioned mixture files (precancerous, stage 1 and stage 2) to be the mixture file. 

3.	I repeated step 2 for each mixture file. I then obtained three resulting files. 

4.	I downloaded the txt files to analyse in R and compute the mean of fractions for each cell type across all samples. I sorted the averages obtained against each cell type and selected the top 5 to show. 

5.	I repeated step 4 for each group and obtained the top 5 average fractions for each cell type per group. 
 

## Observations on Average Immune Cell Type Fractions: 

If we compare the top most prevalent cell types across all groups together:

| Cell Type                      | Fraction Avg - Precancerous Group | Fraction Avg - Stage 1 Non-Invasive Group | Fraction Avg - Stage 2 Invasive Group |
|--------------------------------|----------------------------------|----------------------------------------|------------------------------------|
| T-cells regulatory            | 0.074                            | 0.135                                  | 0.092                              |
| Macrophages M2                | 0.122                            | 0.0998                                 | 0.0916                             |
| T-cells CD4 memory resting    | 0.127                            | 0.100                                  | 0.086                              |
| T-cells CD4 memory activated  | n/a                              | 0.101                                  | n/a                                |
| Mast cells resting            | 0.080                            | n/a                                    | 0.714                              |
| T-cells CD8                   | 0.074                            | n/a                                    | n/a                                |
| Dendritic cells activated     | n/a                              | 0.132                                  | 0.130                              |


### From the table above, the following patterns are observed:

- Across all groups, the most commonly prevalent cell types are Regulatory T cells, Macrophages m2, Tcells CD4 memory resting. 
- T cells CD4 (memory resting) consistently decrease in fraction average from precancerous to stage 1 to stage 2 tumor samples. This could suggest that these cells consistently deplete as the tumor grows and the cancer stages progress. 
- Macrophages decrease in fraction average from precancerous stage to stage 1 and also from stage 1 to stage 2. This could again suggest that this cell type continues to deteriorate in the immuno-oncological environment of the tumor.
- Regulatory T cells increase in average fraction from precancerous to stage 1 tumor samples, and then decrease from stage 1 to stage 2 tumor samples
