# Identifying Genetic Biomarkers for Bladder Cancer

## Project Objectives
This project aims to analyze molecular changes at different stages of bladder cancer, specifically comparing gene expression and immune cell composition across precancerous, Stage 1 Non-Invasive, and Stage 2 Invasive bladder cancer samples. The study focuses on:

- (Step 1) Identifying differentially expressed genes (DGE) between different stages.
- (Step 2) Performing enrichment analysis to determine significant biological pathways.
- (Step 3) Using CIBERSORT to analyze immune cell composition across stages.
- (Step 4) Connecting pathway alterations with immune cell interactions to understand mechanisms of bladder cancer progression and recurrence.

## Methodology
1. **Differential Gene Expression (DGE) Analysis:**
   - Compared Stage 2 Invasive vs. Stage 1 Non-Invasive samples.
   - Compared Stage 1 Non-Invasive vs. Precancerous samples.
   - Identified significantly differentially expressed genes.

2. **Enrichment Analysis:**
   - Used Reactome and Gene Ontology (GO) databases.
   - Identified key pathways impacted by differential gene expression.

3. **CIBERSORT-based Immuno-Oncology Analysis:**
   - Analyzed immune cell composition in different cancer stages.
   - Identified top immune cell types based on fraction averages.

4. **Comparative Analysis and Visualization:**
   - Created bar charts, stacked bar charts, and line graphs using R.
   - Mapped immune cell activity to enriched pathways.
   - Highlighted connections between ECM remodeling, apoptosis regulation, and immune system interactions.

## Folder Structure
```
├── Precancer vs Stage1/                # DGE and Enrichment Analysis for Precancer vs Stage 1 Cancer Data
├── Stage1 vs Stage2/            # DGE and Enrichment Analysis for Stage 1 and Stage 2 Bladder Cancer Data 
├── CIBERSORT_Results/              # CIBERSORT analysis for Precancerous, Stage 1 and Stage 2 Data 
├── Visual_Results/              # Visualization outputs including bar graphs, stacked plots, and line graphs
├── ProjectPresentation.pptx    # Final Presentation on the project concluding insights and potential for future work 
├── ProjectSummary.docx     # Project Documentation and Steps 
└── README.md       # Project guide for github
```

## Replication Instructions

To replicate the analysis:

1. Clone the repository and navigate to the project directory.
   ```sh 
   git clone git@github.com:Tzeene1459/DGE-and-Enrichment-Analysis-for-Bladder-Cancer-Patients.git
   cd DGE-and-Enrichment-Analysis-for-Bladder-Cancer-Patients
   ```
2. Ensure you have R and required libraries installed (DESeq2, edgeR, CIBERSORT, ggplot2, etc.).
3. Run the group comparison analysis using the provided R scripts in this order:
   - Precancer vs Stage 1 
        - Group Comparison 
        - Enrichment Analysis 
   - Stage 1 vs Stage 2
        - Group Comparison 
        - Enrichment Analysis 
4. Execute CIBERSORT immune cell analysis for each stage:
   - Precancerous
   - Stage 1
   - Stage 2
5. View or generate your own visualizations for this project. 
6. Review Documentation and Presentation for this project. 
7. Review Visual_Results/Out_Ciber_BladderCancer_final_LinePlot.pdf for a complete picture of what the analysis looked like when this entire project was repeated for all stages of bladder cancer. 

---

This project serves as a foundational step in understanding the immune microenvironment and genetic alterations in bladder cancer progression.


## Author 
Tazeen Shaukat 