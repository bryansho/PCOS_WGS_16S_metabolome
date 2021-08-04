QIIME 2 Analysis

Details of the QIIME 2 [1] commands used to process the 16S data and produce the Sequence Variant (SV) tables and the clustered SV tables for Ho et al. "Gut metabolites are more predictive of disease- and cohoused- states than gut bacterial features in a mouse model of polycystic ovary syndrome" can be found in the Qiime_2.rtf file. This script was run via Amazon Web Services (AWS). SVs were analyzed unclustered and (SV_Not_Clustered) and clustered at the 97% level which is equivalent to the "genus-level" clustering (SV_Clustered).

Scripts for all the analyses can be found in the folders SV_Clustered and SV_Not_Clustered, and these include CAPs, DESeq2 and Random Forest.

The supplementary tables below show summary statistics for the CAPs and Random Forest analyses along with the 16S OTU results show in the manuscript for comparison. 

<img width="871" alt="image" src="https://user-images.githubusercontent.com/20593241/128244056-842cffd1-55a2-4f81-9690-1b15b1d520db.png">


<img width="912" alt="image" src="https://user-images.githubusercontent.com/20593241/128244263-2857feea-05a1-4f42-b09c-af241e77552a.png">

<img width="561" alt="image" src="https://user-images.githubusercontent.com/20593241/128261748-7a35c6f9-28be-44b6-a0d7-060e050fb0d4.png">
<img width="557" alt="image" src="https://user-images.githubusercontent.com/20593241/128261778-eab6fbf3-370e-437d-aeaf-ec2e0acd4e12.png">


REFERENCES

[1] Bolyen E, Rideout JR, Dillon MR, Bokulich NA, Abnet CC, Al-Ghalith GA, Alexander H, Alm EJ, Arumugam M, Asnicar F, Bai Y, Bisanz JE, Bittinger K, Brejnrod A, Brislawn CJ, Brown CT, Callahan BJ, Caraballo-Rodríguez AM, Chase J, Cope EK, Da Silva R, Diener C, Dorrestein PC, Douglas GM, Durall DM, Duvallet C, Edwardson CF, Ernst M, Estaki M, Fouquier J, Gauglitz JM, Gibbons SM, Gibson DL, Gonzalez A, Gorlick K, Guo J, Hillmann B, Holmes S, Holste H, Huttenhower C, Huttley GA, Janssen S, Jarmusch AK, Jiang L, Kaehler BD, Kang KB, Keefe CR, Keim P, Kelley ST, Knights D, Koester I, Kosciolek T, Kreps J, Langille MGI, Lee J, Ley R, Liu YX, Loftfield E, Lozupone C, Maher M, Marotz C, Martin BD, McDonald D, McIver LJ, Melnik AV, Metcalf JL, Morgan SC, Morton JT, Naimey AT, Navas-Molina JA, Nothias LF, Orchanian SB, Pearson T, Peoples SL, Petras D, Preuss ML, Pruesse E, Rasmussen LB, Rivers A, Robeson MS, Rosenthal P, Segata N, Shaffer M, Shiffer A, Sinha R, Song SJ, Spear JR, Swafford AD, Thompson LR, Torres PJ, Trinh P, Tripathi A, Turnbaugh PJ, Ul-Hasan S, van der Hooft JJJ, Vargas F, Vázquez-Baeza Y, Vogtmann E, von Hippel M, Walters W, Wan Y, Wang M, Warren J, Weber KC, Williamson CHD, Willis AD, Xu ZZ, Zaneveld JR, Zhang Y, Zhu Q, Knight R, and Caporaso JG. 2019. Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology 37: 852–857. https://doi.org/10.1038/s41587-019-0209-9 
