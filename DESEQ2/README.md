# Description
 Differential expression comparisons using DESEq2 for all 3 datasets:1) Metabolites, 2) 16S, and 3) WGS. The metabolites data was split into 2 parts. The first part includes only bile aicds, and the 2nd part includes everything not bile acid. For both 16S and WGS microbial expression was examined. Expression was examined at both 2 and 5 between Placebo (P) vs. Letrozole (LET) and Letrozle vs. Cohoused-Letrozole (LET<sup>ch</sup>). 
 
# Bile acids
    log2fold.ipynb = Jupyter notebook that includes analysis for creating DESEQ2 analysis for the bile acids dataset
    Mapping_file_w_og.csv = bile acids Mapping file
    cohouse_non_mapping.csv = Mapping file treating LET-LET/P-P as one group and LET-P/P-LET as another
    Bile_Acids_Cutoff.csv = count data for all weeks for bile acids
    taxonomy_cutoff.csv  = bile acids taxonomy mapping file

# Metabolites_No_BA
    log2fold_metabolites.ipynb = Jupyter notebook that includes analysis for creating DESEQ2 analysis for the metabolites with no bile acids dataset
    Mapping_file_w_og.csv = metabolites with no bile acids Mapping file
    cohouse_non_mapping.csv = Mapping file treating LET-LET/P-P as one group and LET-P/P-LET as another
    Known_Cutoff_no_BA.csv = count data for all weeks for metabolites with no bile acids
    taxonomy_cutoff_no_BA.csv  = metabolites with no bile acids taxonomy mapping file   

# WGS (T2/T5, both time point follows same file structure)
    Deseq2_T5_mapping.csv = Sample mapping file
    T5_filtered_deseq2.ipynb = Jupyter notebook with DESEq2 execution
    T5_filtered_greater_00001.csv = T5 centrifuge microbial counts
    T5_filtered_greater_00001_CoLvL_deseq.csv = DESEq2 T5 LET<sup>ch</sup> vs. LET comparison
    T5_filtered_greater_00001_PvL_deseq.csv  = DESEq2 T5 P vs. LET comparison
    T5_filtered_log2fold_graph.ipynb = Jupyter notebook to generate DESEq2 result graph
    
# 16S (T2/T5, both time point follows same file structure)
    mapping_file_cohousing2018.tsv  = Sample mapping file
    Deseq2.ipynb  = Jupyter notebook with DESEq2 execution
    otu_table_no_singleton-json.biom = T5 OTU biom table
    rep_set.tre = Tree file
    lvcol_t5.csv = DESEq2 T5 LET<sup>ch</sup> vs. LET comparison
    pvl_t5.csv  = DESEq2 T5 P vs. LET comparison
    Deseq2_Plot.ipynb  = Jupyter notebook to generate DESEq2 result graph
