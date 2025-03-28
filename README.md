# oud_transcriptomics
**BENG 204 Systems Medicine - Winter 2025 - Group Project**

**Understanding Transcriptomic Effects of Opioid Exposure Across Neurodevelopmental Stages in Organoid Models**

Opioid use disorder (OUD) is a crisis that affects millions of people in the United States. Here we analyze transcriptomics data from two human induced pluripotent stem cell (hiPSC)-derived organoid models to investigate the effects of opioid exposure on gene expression during early stage development (Kim et al 2024) and adulthood (Ho et al 2024). Differential expression analysis, functional enrichment analysis (overrepresentation analysis and gene set enrichment analysis), and transcription factor activity inference were performed on the Kim et al single-cell RNA-seq dataset (GEO GSE260711) and Ho et al bulk RNA-seq dataset (GEO GSE210206). Our findings indicate that opioid exposure may affect certain transcription factors and pathways related to brain function and sexual development, with greater disruption of normal brain activity in the developing brain and greater sex-specific effects in the adult brain. The notebooks in this repository contain figures and analysis for our presentation and written report.

Packages and Methods:
-  `scanpy` - QC, preprocessing, and differential expression analysis on Kim scRNA-seq dataset
-  `symphonypy` - cell type annotation for Kim scRNA-seq dataset
-  `decoupler` - generating pseudobulk representation of Kim scRNA-seq dataset, transcription factor activity inference on Kim pseudobulk and Ho bulk datasets
-  `PyDESeq2` - differential expression analysis on Ho bulk dataset and Kim pseudobulk dataset
-  `gseapy` - overrepresentation analysis and gene set enrichment analysis on Kim single-cell, Kim pseudobulk, and Ho bulk datasets

References: 

Kim, H. S., Xiao, Y., Chen, X., He, S., Im, J., Willner, M. J., Finlayson, M. O., Xu, C., Zhu, H., Choi, S. J., Mosharov, E. V., Kim, H., Xu, B., & Leong, K. W. (2024). Chronic opioid treatment arrests neurodevelopment and alters synaptic activity in human midbrain organoids. Advanced Science, 11(21).

Ho, M., Zhang, C., Moon, I., Zhu, X., Coombes, B. J., Biernacka, J., Skime, M., Oesterle, T. S., Karpyak, V. M., Schmidt, K., Gliske, K., Ngo, Q., Skillon, C., Seppala, M. D., Li, H., & Weinshilboum, R. M. (2024). Single cell transcriptomics reveals distinct transcriptional responses to oxycodone and buprenorphine by iPSC-derived brain organoids from patients with opioid use disorder. Molecular Psychiatry, 29(6), 1636–1646.
