# UO BGMP spatial 'omics workshop 2026

Author: Cameron Watson

This repo is intended to aggregate materials for a brief, introductory spatial 'omics workshop for students in the University of Oregon
Bioinformatics and Genomics Master's Program. The workshop nor the repo are comprehensive, instead these are intended as a very brief and high-level introduction to spatial proteomics and spatial transcroptomics analysis. Materials from external sources, such as figures from publications, public datasets, and tutorials, are cited in slides and notebooks where they appear, and a list of all references cited can be found at the bottom of this page. 

---

### Running the notebooks

An `environment.yml` is included with only essential packages pinned at the versions used when developing the notebooks.

The most important package versions to be aware of are: 

```
anndata==0.12.10
scanpy==1.12
spatialdata==0.7.2
spatialdata-io==0.6.0
spatialdata-plot==0.2.14
squidpy==1.8.1
```

As behavior can change quite a bit with different versions

---

### Links to public datasets

*CycIF of Healthy Human Tonsil tissue (Day 1)*

- Original dataset can be accessed from the Human Tumor Atlas Network data portal: https://humantumoratlas.org/ 

- The specific feature table (`cycif_tonsil.csv`) used in this notebook can be downloaded from this public Galaxy history: 

https://cancer.usegalaxy.org/u/watsocam/h/bgmp-spatial-omics-demo-tonsil-cycif 

The Galaxy history also has Vitessce dashboards that can be used to view the image, segmentation mask, and downstream quantified data

*10x Genomics Visium and Xenium of breast cancer serial sections (Day 2)*

- Original publication describing the dataset: https://doi.org/10.1038/s41467-023-43458-x 

- Accessed via SpatialData spatial omics datasets: https://spatialdata.scverse.org/en/stable/tutorials/notebooks/datasets/README.html 
    - Visium dataset name: `visium_associated_xenium_io` (For the notebook, this is stored in current working directory under `datasets/visium/data.zarr`)
    - Xenium dataset name: `xenium_rep1_io` (For the notebook, this is stored in current working directory under `datasets/xenium/data.zarr`)

- Link to download scRNA-seq reference dataset (originally from **Wu et al. (2021)** *Nature Genetics*) for Xenium cell-type annotation can be found in this notebook: 

https://github.com/scverse/spatialdata-notebooks/blob/main/notebooks/paper_reproducibility/00_xenium_and_visium.ipynb 

For the notebook, this is stored in current working directory under `datasets/sc_atlas/BC_atlas_xe.h5ad`

---

### Recommended resources

- Anndata documentation: https://anndata.readthedocs.io/en/stable/ 
- Scanpy documentation: https://scanpy.readthedocs.io/en/stable/ 
- SpatialData documentation: https://spatialdata.scverse.org/en/stable/ 
- napari documentation: https://napari.org/stable/ 


---

### References

*Day 1 slides*

- Moskal K, Puchta-Jasińska M, Bolc P, Motor A, Frankowski R, Pietrusińska-Radzio A, Rucińska A, Tomiczak K, Boczkowska M. Why "Where" Matters as Much as "How Much": Single-Cell and Spatial Transcriptomics in Plants. Int J Mol Sci. 2025 Dec 7;26(24):11819. doi: 10.3390/ijms262411819. PMID: 41465249; PMCID: PMC12732828.

- Lee TA, Illouz-Eliaz N, Nobori T, Xu J, Jow B, Nery JR, Ecker JR. A single-cell, spatial transcriptomic atlas of the Arabidopsis life cycle. Nat Plants. 2025 Sep;11(9):1960-1975. doi: 10.1038/s41477-025-02072-z. Epub 2025 Aug 19. PMID: 40830271; PMCID: PMC12416547.

- Hussein IH, Raad M, Safa R, Jurjus R, Jurjus A (2015) Once Upon a Microscopic Slide: The Story of Histology. J Cytol Histol 6:377. doi:10.4172/2157-7099.1000377

- Alberts B, Johnson A, Lewis J, et al. Molecular Biology of the Cell. 4th edition. New York: Garland Science; 2002. Looking at the Structure of Cells in the Microscope. Available from: https://www.ncbi.nlm.nih.gov/books/NBK26880/

- Epstein, J. Prostate cancer grading: a decade after the 2005 modified system. Mod Pathol 31 (Suppl 1), 47–63 (2018). https://doi.org/10.1038/modpathol.2017.133

- SEER Training Modules: Morphology & Grade. U.S. National Institutes of Health, National Cancer Institute. Cited 19 February 2026. Available from: https://training.seer.cancer.gov.

- Focke CM, Decker T, van Diest PJ. The reliability of histological grade in breast cancer core needle biopsies depends on biopsy size: a comparative study with subsequent surgical excisions. Histopathology. 2016 Dec;69(6):1047-1054. doi: 10.1111/his.13036. Epub 2016 Sep 23. PMID: 27417415.

- Sjödahl G, Lövgren K, Lauss M, Chebil G, Patschan O, Gudjonsson S, Månsson W, Fernö M, Leandersson K, Lindgren D, Liedberg F, Höglund M. Infiltration of CD3⁺ and CD68⁺ cells in bladder cancer is subtype specific and affects the outcome of patients with muscle-invasive tumors. Urol Oncol. 2014 Aug;32(6):791-7. doi: 10.1016/j.urolonc.2014.02.007. Epub 2014 Apr 29. PMID: 24794251.

- Method of the Year 2024: spatial proteomics. Nat Methods. 2024 Dec;21(12):2195-2196. doi: 10.1038/s41592-024-02565-3. PMID: 39643689.

- Bodenmiller B. Highly multiplexed imaging in the omics era: understanding tissue structures in health and disease. Nat Methods. 2024 Dec;21(12):2209-2211. doi: 10.1038/s41592-024-02538-6. PMID: 39643676.

- Blise, K.E., Sivagnanam, S., Banik, G.L. et al. Single-cell spatial architectures associated with clinical outcome in head and neck squamous cell carcinoma. npj Precis. Onc. 6, 10 (2022). https://doi.org/10.1038/s41698-022-00253-z

- Semba T, Ishimoto T. Spatial analysis by current multiplexed imaging technologies for the molecular characterisation of cancer tissues. Br J Cancer. 2024 Dec;131(11):1737-1747. doi: 10.1038/s41416-024-02882-6. Epub 2024 Oct 22. PMID: 39438630; PMCID: PMC11589153.

- Bernas T, Grégori G, Asem EK, Robinson JP. Integrating cytomics and proteomics. Mol Cell Proteomics. 2006 Jan;5(1):2-13. doi: 10.1074/mcp.R500014-MCP200. Epub 2005 Oct 28. PMID: 16258168.

- Lin JR, Fallahi-Sichani M, Chen JY, Sorger PK. Cyclic Immunofluorescence (CycIF), A Highly Multiplexed Method for Single-cell Imaging. Curr Protoc Chem Biol. 2016 Dec 7;8(4):251-264. doi: 10.1002/cpch.14. PMID: 27925668; PMCID: PMC5233430.

- Muhlich JL, Chen YA, Yapp C, Russell D, Santagata S, Sorger PK. Stitching and registering highly multiplexed whole-slide images of tissues and tumors using ASHLAR. Bioinformatics. 2022 Sep 30;38(19):4613-4621. doi: 10.1093/bioinformatics/btac544. PMID: 35972352; PMCID: PMC9525007.

- Schapiro D, Sokolov A, Yapp C, Chen YA, Muhlich JL, Hess J, Creason AL, Nirmal AJ, Baker GJ, Nariya MK, Lin JR, Maliga Z, Jacobson CA, Hodgman MW, Ruokonen J, Farhi SL, Abbondanza D, McKinley ET, Persson D, Betts C, Sivagnanam S, Regev A, Goecks J, Coffey RJ, Coussens LM, Santagata S, Sorger PK. MCMICRO: a scalable, modular image-processing pipeline for multiplexed tissue imaging. Nat Methods. 2022 Mar;19(3):311-315. doi: 10.1038/s41592-021-01308-y. Epub 2021 Nov 25. PMID: 34824477; PMCID: PMC8916956.

- Guo, N., Xiong, W., Wu, Q., Jing, N., 2016. An efficient tile-pyramids building method for fast visualization of massive geospatial raster datasets. Advances in Electrical and Computer Engineering 16 (4), 3-8.
Available from: URL: http://dx.doi.org/10.4316/AECE.2016.04001

- Moore, J., Allan, C., Besson, S. et al. OME-NGFF: a next-generation file format for expanding bioimaging data-access strategies. Nat Methods 18, 1496–1498 (2021). https://doi.org/10.1038/s41592-021-01326-w

- Moore J, Basurto-Lozada D, Besson S, Bogovic J, Bragantini J, Brown EM, Burel JM, Moreno XC, de Medeiros G, Diel EE, Gault D, Ghosh SS, Gold I, Halchenko YO, Hartley M, Horsfall D, Keller MS, Kittisopikul M, Kovacs G, Yoldaş AK, Kyoda K, de la Villegeorges ALT, Li T, Liberali P, Lindner D, Linkert M, Lüthi J, Maitin-Shepard J, Manz T, Marconato L, McCormick M, Lange M, Mohamed K, Moore W, Norlin N, Ouyang W, Özdemir B, Palla G, Pape C, Pelkmans L, Pietzsch T, Preibisch S, Prete M, Rzepka N, Samee S, Schaub N, Sidky H, Solak AC, Stirling DR, Striebel J, Tischer C, Toloudis D, Virshup I, Walczysko P, Watson AM, Weisbart E, Wong F, Yamauchi KA, Bayraktar O, Cimini BA, Gehlenborg N, Haniffa M, Hotaling N, Onami S, Royer LA, Saalfeld S, Stegle O, Theis FJ, Swedlow JR. OME-Zarr: a cloud-optimized bioimaging file format with international community support. bioRxiv [Preprint]. 2023 May 7:2023.02.17.528834. doi: 10.1101/2023.02.17.528834. Update in: Histochem Cell Biol. 2023 Sep;160(3):223-251. doi: 10.1007/s00418-023-02209-1. PMID: 36865282; PMCID: PMC9980008.

- Stringer, C., Wang, T., Michaelos, M. et al. Cellpose: a generalist algorithm for cellular segmentation. Nat Methods 18, 100–106 (2021). https://doi.org/10.1038/s41592-020-01018-x

- Virshup et al., (2024). anndata: Access and store annotated data matrices. Journal of Open Source Software, 9(101), 4371, https://doi.org/10.21105/joss.04371

- Johnson BE, Creason AL, Stommel JM, Keck JM, Parmar S, Betts CB, Blucher A, Boniface C, Bucher E, Burlingame E, Camp T, Chin K, Eng J, Estabrook J, Feiler HS, Heskett MB, Hu Z, Kolodzie A, Kong BL, Labrie M, Lee J, Leyshock P, Mitri S, Patterson J, Riesterer JL, Sivagnanam S, Somers J, Sudar D, Thibault G, Weeder BR, Zheng C, Nan X, Thompson RF, Heiser LM, Spellman PT, Thomas G, Demir E, Chang YH, Coussens LM, Guimaraes AR, Corless C, Goecks J, Bergan R, Mitri Z, Mills GB, Gray JW. An omic and multidimensional spatial atlas from serial biopsies of an evolving metastatic breast cancer. Cell Rep Med. 2022 Feb 15;3(2):100525. doi: 10.1016/j.xcrm.2022.100525. PMID: 35243422; PMCID: PMC8861971.

*Day 1 notebook*

- Rozenblatt-Rosen et al. The Human Tumor Atlas Network: Charting Tumor Transitions across Space and Time at Single-Cell Resolution. Cell 2020 Apr 16;181(2):236-249. Pubmed: https://pubmed.ncbi.nlm.nih.gov/32302568/ Cell: https://doi.org/10.1016/j.cell.2020.03.053.

- de Bruijn, I., Nikolov, M., Lau, C. et al. Sharing data from the Human Tumor Atlas Network through standards, infrastructure and community engagement. Nat Methods (2025). Nat Methods: https://doi.org/10.1038/s41592-025-02643-0

- Wolf FA, Angerer P, Theis FJ. SCANPY: large-scale single-cell gene expression data analysis. Genome Biol. 2018 Feb 6;19(1):15. doi: 10.1186/s13059-017-1382-0. PMID: 29409532; PMCID: PMC5802054.

- Palla G, Spitzer H, Klein M, Fischer D, Schaar AC, Kuemmerle LB, Rybakov S, Ibarra IL, Holmberg O, Virshup I, Lotfollahi M, Richter S, Theis FJ. Squidpy: a scalable framework for spatial omics analysis. Nat Methods. 2022 Feb;19(2):171-178. doi: 10.1038/s41592-021-01358-2. Epub 2022 Jan 31. PMID: 35102346; PMCID: PMC8828470.

*Day 2 slides*

- Felipe Segato Dezem, Wani Arjumand, Hannah DuBose, Natalia Silva Morosini, Jasmine Plummer. 2024. Spatially Resolved Single-Cell Omics: Methods, Challenges, and Future Perspectives. Annual Review Biomedical Data Science. 7:131-153. https://doi.org/10.1146/annurev-biodatasci-102523-103640

- Chen WT, Lu A, Craessaerts K, Pavie B, Sala Frigerio C, Corthout N, Qian X, Laláková J, Kühnemund M, Voytyuk I, Wolfs L, Mancuso R, Salta E, Balusu S, Snellinx A, Munck S, Jurek A, Fernandez Navarro J, Saido TC, Huitinga I, Lundeberg J, Fiers M, De Strooper B. Spatial Transcriptomics and In Situ Sequencing to Study Alzheimer's Disease. Cell. 2020 Aug 20;182(4):976-991.e19. doi: 10.1016/j.cell.2020.06.038. Epub 2020 Jul 22. PMID: 32702314.

- Chen TY, You L, Hardillo JAU, Chien MP. Spatial Transcriptomic Technologies. Cells. 2023 Aug 10;12(16):2042. doi: 10.3390/cells12162042. PMID: 37626852; PMCID: PMC10453065.

- Plummer, J.T., Dezem, F.S., Cook, D.P. et al. Standardized metrics for assessment and reproducibility of imaging-based spatial transcriptomics datasets. Nat Biotechnol (2025). https://doi.org/10.1038/s41587-025-02811-9

- Ospina OE, Manjarres-Betancur R, Gonzalez-Calderon G, Soupir AC, Smalley I, Tsai KY, Markowitz J, Khaled ML, Vallebuona E, Berglund AE, Eschrich SA, Yu X, Fridley BL. spatialGE Is a User-Friendly Web Application That Facilitates Spatial Transcriptomics Data Analysis. Cancer Res. 2025 Mar 3;85(5):848-858. doi: 10.1158/0008-5472.CAN-24-2346. PMID: 39636739; PMCID: PMC11873723.

- Cable DM, Murray E, Zou LS, Goeva A, Macosko EZ, Chen F, Irizarry RA. Robust decomposition of cell type mixtures in spatial transcriptomics. Nat Biotechnol. 2022 Apr;40(4):517-526. doi: 10.1038/s41587-021-00830-w. Epub 2021 Feb 18. PMID: 33603203; PMCID: PMC8606190.

- Miller, B.F., Huang, F., Atta, L. et al. Reference-free cell type deconvolution of multi-cellular pixel-resolution spatially resolved transcriptomics data. Nat Commun 13, 2339 (2022). https://doi.org/10.1038/s41467-022-30033-z

- Janesick A, Shelansky R, Gottscho AD, Wagner F, Williams SR, Rouault M, Beliakoff G, Morrison CA, Oliveira MF, Sicherman JT, Kohlway A, Abousoud J, Drennon TY, Mohabbat SH; 10x Development Teams; Taylor SEB. High resolution mapping of the tumor microenvironment using integrated single-cell, spatial and in situ analysis. Nat Commun. 2023 Dec 19;14(1):8353. doi: 10.1038/s41467-023-43458-x. PMID: 38114474; PMCID: PMC10730913.

*Day 2 notebook*

- Marconato, L., Palla, G., Yamauchi, K.A. et al. SpatialData: an open and universal data framework for spatial omics. Nat Methods 22, 58–62 (2025). https://doi.org/10.1038/s41592-024-02212-x

- Chi-Li Chiu, Nathan Clack, the napari community, napari: a Python Multi-Dimensional Image Viewer Platform for the Research Community, Microscopy and Microanalysis, Volume 28, Issue S1, 1 August 2022, Pages 1576–1577, https://doi.org/10.1017/S1431927622006328

- Wu, S.Z., Al-Eryani, G., Roden, D.L. et al. A single-cell and spatially resolved atlas of human breast cancers. Nat Genet 53, 1334–1347 (2021). https://doi.org/10.1038/s41588-021-00911-1