# Descirption
CAPs analysis of beta-diversity using bray-curtis dissimilarity. Three data sets were used: 1) Gut Metabolites, 2) Gut 16S sequencing, and 3) WGS metagenome. PERMANOVA (999 permutations) was used to evaluate differentiation between treatments. 

## File mapping

### Seperate Folder (Includes files for individual CAP analysis)
  - 16s_map.csv = 16S mapping file. Includes sample ID associated with timepoint and treatment.
  - CAP.ipynb = Jupyter notebook that includes analysis for creating CAPs analysis for Metabolite (week 0 - week 5), 16S (week 2 and 5), WGS (week 2 and 5)
  - Mapping_file_w_og.csv = WGS and metabolite mapping file. Includes meta data for each sample
  - T2_filtered_greater_00001.csv = Week 2 WGS centrifuge microbial taxonomy count data
  - T5_filtered_greater_00001.csv = Week 5 WGS centrifuge microbial taxonomy count data
  - Unknown_Cutoff.csv = Metabolite count data
  - otu_table_alltime_w_category.tsv = 16S QIIME taxonomy count data
  - taxonomy.csv = Metabolite taxonomy mapping file
  - taxonomy_16s.csv = 16S microbial taxonomy mapping file
  - taxonomy_centrifuge.csv = WGS microbial taxonomy file 

### Combined (Includes files for the multi-omic CAP analysis)
  - CAP Combined.ipynb = Jupyter notebook that includes analysis for creating CAPs analysis for the 2 multi-omics dataset: 1)Metabolome and 16S, and 2)Metabolome and WGS
  - Deseq2_T2_mapping.csv = WGS week 2 sample mapping file 
  - Deseq2_T5_mapping.csv = WGS week 5 sample mapping file
  - Mapping_file_w_og.csv = Metabolite Mapping file
  - Metabolites_16S.csv = Week 2 and 5 combined metabolite and 16S count data
  - T2_Metabolites_WGS.csv = Week 2 combined metabolite and WGS data
  - T5_Metabolites_WGS.csv = Week 5 combined metabolite and WGS data
  - taxonomy_metabolites_16S.csv = Metabolite and 16S taxonomy mapping file 
  - taxonomy_metabolites_WGS.csv = Metabolite and WGS taxonomy mapping file
  
  ### Permanova Folder (Includes files for individual CAP analysis)
  #### 16S
  - sckitbio_permanova.ipynb = Jupyter notebook that includes Permanova analysis for 16S (week 2 and 5)
  - otu_table_T2.tsv = Week 2 16s taxonomy count data
  - otu_table_T5.tsv = Week 5 16s taxonomy count data
  - mapping_file_cohousing2018.tsv = 16S QIIME Mapping file
  #### WGS
  ##### T2/T5 (Both directory follow same file structure)
  - Permanova_T2_Centrifuge.ipynb = Jupyter notebook that includes Permanova analysis for WGS (week 2/week 5)
  - Deseq2_T2_mapping.csv = WGS Week 2 mapping file. Includes meta data for each sample (week 2/week 5)
  - Permanova_T2_filtered_greater_00001.csv = WGS Week 2 count data (week 2/week 5)
  #### Metabolite + WGS
  ##### T2/T5 (Both directory follow same file structure)
  - Deseq2_T2_mapping.csv = Sample Mapping file 
  - Permanova_T2_Omics.ipynb = Jupyter notebook for PERMANOVA analysis
  - T2_Metabolites_WGS.csv = Combined count data
