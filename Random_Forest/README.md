# Description
Random forest on multi-omics and independent dataset. Only include top 10 results from DESEq2.

# Multi-omics
## T2/T5 (Same file structure)
  - T2_RF_Top_Log2fold.ipynb = Jupyter notebook with multi-omics random forest execution 
  - T2_Known_WSG_PvL.csv = Placebo vs. Letrozle Metabolites and WGS dataset 
  - T2_WSG_BA_PvL.csv = Placebo vs. Letrozole Bile acids and WGS dataset 
  - T2_Known_WSG_LvCoL.csv = Letrozole vs. Cohoused-letrozole Metabolites and WGS dataset 
  - T2_WSG_BA_LvCoL.csv = Letrozole vs. Cohoused-letrozole Bile acids and WGS dataset
## 16S+BA (Same file structure)
  - RandomForest_16S+BA.ipynb  = Jupyter notebook with multi-omics only Bile Acid random forest execution 
  - RandomForest_Metabolite+16S.ipynb  = Jupyter notebook with multi-omics random forest execution
  - merge_denovo_Known_no_BA_t2pvl.csv = Placebo vs. Letrozle Metabolites and 16S dataset 
  - merge_denovo_BAlim_t2pvl.csv = Placebo vs. Letrozole Bile acids and 16S dataset 
  - merge_denovo_Known_no_BA_t2lvcol.csv = Letrozole vs. Cohoused-letrozole Metabolites and 16S dataset 
  - merge_denovo_BAlim_t2lvcol.csv = Letrozole vs. Cohoused-letrozole Bile acids and 16S dataset
  - RF_Feature_graph_16S+BA.ipynb = graph all random forest results
  - RF_top_features.csv = all random forest results
  

# Independent Dataset
## T2/T5 (Same file structure)
  - T2_RF_Individual_data_set.ipynb = Jupyter notebook with independent random forest execution
  - T2_BA_LvCoL.csv = Letrozole vs Cohoused-letrozole bile acid dataset 
  - T2_BA_PvL.csv = Placebo vs. Letrozole Bile acids dataset
  - T2_Known_LvCoL.csv = Letrozole vs Cohoused-letrozole metabolite dataset
  - T2_Known_PvL.csv = Placebo vs. Letrozole metabolite dataset
  - T2_WSG_LvCoL.csv = Letrozole vs Cohoused-letrozole WGS dataset
  - T2_WSG_PvL.csv = Placebo vs. Letrozole WGS dataset

# Graphing results
  - RF_Feature_graph.ipynb = graph all random forest results
  - RF_top_features.csv = all random forest results
