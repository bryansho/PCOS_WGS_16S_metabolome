QIIME 2 Analysis

Details of the QIIME 2 commands used to process the 16S data and produce the Sequence Variant (SV) tables and the clustered SV tables for Ho et al. "Gut metabolites are more predictive of disease- and cohoused- states than gut bacterial features in a mouse model of polycystic ovary syndrome" can be found in the Qiime_2.rtf file. This script was run via Amazon Web Services (AWS). SVs were analyzed unclustered and (SV_Not_Clustered) and clustered at the 97% level which is equivalent to the "genus-level" clustering (SV_Clustered).

Scripts for all the analyses can be found in the folders SV_Clustered and SV_Not_Clustered, and these include CAPs, DESeq2 and Random Forest.

The supplementary tables below show summary statistics for the CAPs and Random Forest analyses along with the 16S OTU results show in the manuscript for comparison. 

Table S1. Comparision of summary statistics for 16S CAP analysis based on amplicon sequence variants (SVs) 					
denoised using DADA2 to the 16S OTU results. The R2 and P-values were determined via PERMANOVA 					
with 999 permutations.					
					
Data  Set	        Time Point	  R2	  P-value (unadjusted)  CAP Variance*	
16S   SV	        2	            0.12	      0.05	            11.30%	
16S   SV 	        5	            0.0 9	      0.69	            7.50%	
16S   SV (97%)**	2	            0.12	      0.06              10.20%	
16S   SV (97%) 	  5	            0.08	      0.65	            9.90%	
16S   OTUs (97%)	2	            0.21	      0.03	            12.90%	
16S   OTUs (97%)	5	            0.17	      0.32	            9.60%	
					
* Fraction of variance explained by the first two principal components of the CAP analysis.					
					
16S SV = Denoised via DADA2 algorithm; no clustering.					
16S SV (97%) = Denoised via DADA2; clustered at the 97% level using vsearch.					
16S OTU (97%) = The results from the manscript, Figure 3 parts C and D.					
					
Table S2. Comparison of random forest results between DADA2 denoised 16S SVs and the 16S OTU data.					
					
Data Set	        Comparison	    Time Point  Accuracy	OOB	
16S SV	          P vs LET	      2	          33%	      90%	
16S SV	          LET vs LETch	  2	          33%	      67%	
16S SV	          P vs LET	      5	          50%	      50%	
16S SV	          LET vs LETch	  5	          40%	      67%	
16S SV (97%) 	    P vs LET	      2	          33%	      50%	
16S SV (97%) 	    LET vs LETch	  2	          33%	      78%	
16S SV (97%) 	    P vs LET	      5	          33%	      40%	
16S SV (97%) 	    LET vs LETch	  5	          40%	      56%	
16S OTUs (97%)	  P vs LET	      2	          83%     	20%	
16S OTUs (97%)	  LET vs LETch	  2	          100%      94%	
16S OTUs (97%)	  P vs LET	      5	          50%	      40%	
16S OTUs (97%)	  LET vs LETch	  5	          40%	      30%	
					
Accuracy = Percentage of correctly classified samples.					
OOB (Out of Bag Score) = Percentage of correctly classified samples based on unselected samples from the bootstrap sampling method.					
