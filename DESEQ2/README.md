# Description
 Differential expression comparisons using DESEq2 for all 3 datasets:1) Metabolites, 2) 16S, and 3) WGS. The metabolites data was split into 2 parts. The first part includes only bile aicds, and the 2nd part includes everything not bile acid. For both 16S and WGS microbial expression was examined. Expression was examined at both 2 and 5 between Placebo (P) vs. Letrozole (LET) and Letrozle vs. Cohoused-Letrozole (LET<sup>ch</sup>). 
 
# Bile acids
    log2fold.ipynb = Jupyter notebook that includes analysis for creating DESEQ2 analysis for the bile acids dataset
    Mapping_file_w_og.csv = bile acids Mapping file
    cohouse_non_mapping.csv = Mapping file treating LET-LET/P-P as one group and LET-P/P-LET as another
    Bile_Acids_Cutoff.csv = count data for all weeks for bile acids
    taxonomy_cutoff.csv  = bile acids taxonomy mapping file
