QIIME 2 Analysis

Details of the QIIME 2 (Bolyn et al. 2019) commands used to process the 16S data and produce the Sequence Variant (SV) tables and the clustered SV tables for Ho et al. "Gut metabolites are more predictive of disease- and cohoused- states than gut bacterial features in a mouse model of polycystic ovary syndrome" can be found in the Qiime_2.rtf file. This script was run via Amazon Web Services (AWS). SVs were analyzed unclustered and (SV_Not_Clustered) and clustered at the 97% level which is equivalent to the "genus-level" clustering (SV_Clustered).

Scripts for all the analyses can be found in the folders SV_Clustered and SV_Not_Clustered, and these include CAPs, DESeq2 and Random Forest.

The supplementary tables below show summary statistics for the CAPs and Random Forest analyses along with the 16S OTU results show in the manuscript for comparison. 

<img width="871" alt="image" src="https://user-images.githubusercontent.com/20593241/128244056-842cffd1-55a2-4f81-9690-1b15b1d520db.png">


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



Bolyen E, Rideout JR, Dillon MR, Bokulich NA, Abnet CC, Al-Ghalith GA, Alexander H, Alm EJ, Arumugam M, Asnicar F, Bai Y, Bisanz JE, Bittinger K, Brejnrod A, Brislawn CJ, Brown CT, Callahan BJ, Caraballo-Rodríguez AM, Chase J, Cope EK, Da Silva R, Diener C, Dorrestein PC, Douglas GM, Durall DM, Duvallet C, Edwardson CF, Ernst M, Estaki M, Fouquier J, Gauglitz JM, Gibbons SM, Gibson DL, Gonzalez A, Gorlick K, Guo J, Hillmann B, Holmes S, Holste H, Huttenhower C, Huttley GA, Janssen S, Jarmusch AK, Jiang L, Kaehler BD, Kang KB, Keefe CR, Keim P, Kelley ST, Knights D, Koester I, Kosciolek T, Kreps J, Langille MGI, Lee J, Ley R, Liu YX, Loftfield E, Lozupone C, Maher M, Marotz C, Martin BD, McDonald D, McIver LJ, Melnik AV, Metcalf JL, Morgan SC, Morton JT, Naimey AT, Navas-Molina JA, Nothias LF, Orchanian SB, Pearson T, Peoples SL, Petras D, Preuss ML, Pruesse E, Rasmussen LB, Rivers A, Robeson MS, Rosenthal P, Segata N, Shaffer M, Shiffer A, Sinha R, Song SJ, Spear JR, Swafford AD, Thompson LR, Torres PJ, Trinh P, Tripathi A, Turnbaugh PJ, Ul-Hasan S, van der Hooft JJJ, Vargas F, Vázquez-Baeza Y, Vogtmann E, von Hippel M, Walters W, Wan Y, Wang M, Warren J, Weber KC, Williamson CHD, Willis AD, Xu ZZ, Zaneveld JR, Zhang Y, Zhu Q, Knight R, and Caporaso JG. 2019. Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology 37: 852–857. https://doi.org/10.1038/s41587-019-0209-9 
