# Cell Migration Lab Datasets

Welcome to the  Cell Migration Lab's datasets repository. Here, you will find a comprehensive list of openly available datasets generated by our lab or by Guillaume Jacquemet before the cell migration lab started.

For any inquiries or further information about these datasets, please get in touch with us!

# Table of Contents
- [Deep Learning training datasets and models](https://github.com/CellMigrationLab/ModelZoo)
- [Materials at Addgene](#Materials-at-Addgene)
- [Proteomic Data](#Proteomic-Data)
- [Sequencing Data](#Sequencing-Data)
- [Image Data](#Image-Data)

# Materials at Addgene

<div style="width: 280px; border: thin solid #888; padding: 10px; text-align: center;"><a href="https://www.addgene.org/Guillaume_Jacquemet/" style="text-decoration: none; color: #585858; font-size: 16px; font-family: Arial,Helvetica,sans-serif;" target="_blank" rel="noopener noreferrer"><b>Guillaume Jacquemet Lab</b><br>Find and request materials through<br><img style="margin-top: 16px;" width="250" height="48" alt="Addgene" src="https://media.addgene.org/cms/filer_public/ea/82/ea826144-fce2-4c13-99e9-940af7e2853b/logo-addgene.png"></a></div>

# Proteomic Data

Our lab has generated and published a series of proteomic datasets focusing on protein interactions and cellular fractionation. Below is a summary of these datasets, providing insights into various proteins and their binding partners in different cellular contexts.

| Dataset Name | Description | View Dataset | Reference |
| ------------ | ----------- | ------------ | --------- |
| TLNRD1-GFP Pulldown in HEK293T Cells | Pulldown of human TLNRD1-GFP and GFP in HEK cells for mass spectrometry analysis of binding partners. | [View Dataset](https://www.ebi.ac.uk/pride/archive/projects/PXD045258) | [Ball et al., 2023](https://www.biorxiv.org/content/10.1101/2023.09.29.559344v1) |
| Talin1-GFP Pulldown in U2OS Cells | Study of human Talin1-GFP and GFP pulldown from U2OS cells plated on fibronectin, using mass spectrometry. | [View Dataset](https://www.ebi.ac.uk/pride/archive/projects/PXD024634) | [Gough et al., 2021](https://www.jbc.org/article/S0021-9258(21)00635-9/fulltext) |
| Sharpin-GFP Pulldown in HEK293T Cells | Analysis of human Sharpin-GFP and GFP pulldown from HEK293T cells, identifying binding partners through mass spectrometry. | [View Dataset](https://www.ebi.ac.uk/pride/archive/projects/PXD004734) | [Khan et al., 2017](https://journals.biologists.com/jcs/article/130/18/3094/56377/The-Sharpin-interactome-reveals-a-role-for-Sharpin) |
| Plasma Membrane, Endosomal, and Cytoplasmic Fractions in Mouse Embryonic Fibroblast | Cellular fractionation experiments to identify novel endosomal proteins in mouse embryonic fibroblast. | [View Dataset](https://www.ebi.ac.uk/pride/archive/projects/PXD001870) | [Alanko et al., 2015](https://www.nature.com/articles/ncb3250) |
| Proteomic analysis of filamin-A, IQGAP1, Rac1 and RCC2 binding partners | Analysis of human filamin-A-GFP, IQGAP1-GFP, Rac1 and RCC2-GFP and GFP pulldown from HEK293T cells, identifying binding partners through mass spectrometry. | [View Dataset](https://www.ebi.ac.uk/pride/archive/projects/PRD000726) | [Jacquemet et al., 2013](https://journals.biologists.com/jcs/article/126/18/4121/53831/Rac1-is-deactivated-at-integrin-activation-sites) |

# Sequencing Data

Our lab has been actively generating and publishing sequencing datasets.

| Dataset Name                                        | Sequencing Type | Description                                                                                                 | View Dataset                                                                 | Reference                                                                    |
|-----------------------------------------------------|-----------------|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| MYO10-Filopodia Breast Tumor Xenograft Expression Dataset | RNA-Seq         | mRNA sequencing data from subcutaneous breast tumor xenografts of MCF10DCIS.com cell lines expressing non-targeting control shRNA (4 tumors) or Myosin-X targeting shRNA (4 tumors). | [View Dataset](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE166898) | [Peuhu et al., 2022](https://www.sciencedirect.com/science/article/pii/S1534580722007134#sec4) |


<!-- Add more rows as needed -->

# Image Data

This section overviews our publicly available image datasets, encompassing various studies. 

## [Fast label-free live imaging reveals key roles of flow dynamics and CD44-HA interaction in cancer cell arrest on endothelial monolayers](https://github.com/CellMigrationLab/PDAC_DL/tree/main)

All data and code associated with the manuscript [Follain et al., 2024](https://www.biorxiv.org/content/10.1101/2024.09.30.615654v1) are available in a dedicated [Zenodo community](https://zenodo.org/communities/pdac_dl) 

| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| Fast label-free live imaging reveals regulation of cancer cell endothelium adhesion by flow and CD44-HA interaction | This repository contains all the data used to make the figure shown in the paper | [View Dataset on Zenodo](https://zenodo.org/records/13846276) | [Follain et al., 2024](https://www.biorxiv.org/content/10.1101/2024.09.30.615654v1) | 

#### Segmentation models
| Model Name | Imaging Modality | Performance | Purpose and Associated Figure | Training Dataset Link |
|------------|------------------|-------------|-------------------------------|-----------------------|
| Flow chamber dataset | Brightfield      | IoU = 0.813 <br> f1 = 0.933 | StarDist model to detect cancer cells in BSA-coated channels. Used to measure perfusion speed inside the channels (Fig S1). | [Link](https://zenodo.org/records/4034939) |
| StarDist_Fluorescent_cells | Fluorescence     | IoU = 0.646 <br> f1 = 0.877 | StarDist model to detect cancer cells from fixed samples. Used in Fig. 1 to count the number of attached cells | [Link](https://doi.org/10.5281/zenodo.10572310) |
| StarDist_BF_cancer_cell_dataset_20x | Brightfield | IoU = 0.793 <br> f1 = 0.921 | StarDist model capable of segmenting cancer cells on endothelial cells (20x magnification). This model was used to segment cancer cells prior to tracking in Fig 1.  | [Link](https://doi.org/10.5281/zenodo.10572122) |
| StarDist_BF_Neutrophil_dataset | Brightfield | IoU = 0.914 <br> f1 = 0.969 | StarDist model capable of segmenting neutrophils on endothelial cells. This model was used to segment neutrophils prior to tracking in Fig 2. | [Link](https://doi.org/10.5281/zenodo.10572231) |
| StarDist_BF_Monocytes_dataset | Brightfield | IoU = 0.831 <br> f1 = 0.941 | StarDist model capable of segmenting mononucleated cells on endothelial cells. This model was used to segment mononucleated cells prior to tracking in Fig 2. | [Link](https://doi.org/10.5281/zenodo.10572200) |
| StarDist_HUVEC_nuclei_dataset | Fluorescence     | IoU = 0.927 <br> f1 = 0.976 | StarDist model capable of segmenting endothelial nuclei while ignoring cancer cells. Used to segment endothelial nuclei in Fig 4. | [Link](https://doi.org/10.5281/zenodo.10617532) |
| StarDist_BF_cancer_cell_dataset_10x | Brightfield     | IoU = 0.882 <br> f1 = 0.968 | StarDist model capable of segmenting cancer cells on endothelial cells (10x magnification). This model used in figure 7, 8 + associated supplementary figures. | [Link](https://zenodo.org/uploads/13304399) |
| StarDist_AsPC1_Lifeact | Fluorescence     | IoU = 0.884 <br> f1 = 0.967 | StarDist model capable of segmenting AsPC1 cells from AsPC1 channel, in addition to segmenting from background, model also segments individual cells from clusters. Used in figure 6.| [Link](https://zenodo.org/records/13442128) |
| Stardist_MiaPaCa2_from_CD44 | Fluorescence     | IoU = 0.884 <br> f1 = 0.950 | StarDist model capable of segmenting MiaPaCa2 cells from CD44 channel while ignoring endothelial cells. Used in figure 6. | [Link](https://doi.org/10.5281/zenodo.13442877) |
| StarDist_TumorCell_nuclei | Fluorescence     | IoU = 0.558 <br> f1 = 0.793 | StarDist model capable of segmenting tumor cell nuclei from the nuclei channel while ignoring endothelial nuclei. | [Link](https://doi.org/10.5281/zenodo.13443221) |

#### Artificial labeling models

| Model Name | Performance | Purpose and Associated Figure | Training Dataset Link |
|------------|-------------|-------------------------------|-----------------------|
| pix2pix_HUVEC_nuclei_cancer_cells_dataset | SSIM = 0.755 <br> lpips = 0.120 | This model was used in Fig. 4 to artificially label nulcei from BF images with cancer and endothelial cells. | [Link](https://doi.org/10.5281/zenodo.10621667) |
| pix2pix_HUVEC_nuclei_immuno_cells_dataset | SSIM = 0.756 <br> lpips = 0.130 | This model was used in Fig. 4 to artificially label nulcei from BF images with immuno and endothelial cells. | [Link](https://doi.org/110.5281/zenodo.10617565) |
| pix2pix_HUVEC_juctions_dataset | SSIM = 0.270 <br> lpips = 0.360 | This model was used in Fig. 4 to artificially label cell-cell juctions from BF images with immuno or cancer and endothelial cells. | [Link](https://doi.org/10.5281/zenodo.10611092) |

#### Tracking datasets
| Dataset name | Purpose and Associated Figure | Link to dataset |
|------------|-------------|-------------------------------|
| PDAC cells vs Immune cells perfusion tracking dataset | This dataset was used to analyze the attachment of PDAC and immune cells to the endothelium in Fig.2, Fig.3 Fig.4 and SFig.5. | [Link to dataset](https://doi.org/10.5281/zenodo.13643590) |
| PDAC cells CD44 siRNA perfusion tracking dataset | This dataset was used to analyze the attachment of PDACs to the endothelium in Fig.7, SFig.7 and SFig8. | [Link to dataset](https://doi.org/10.5281/zenodo.13379627) |
| HUVEC CD44 siRNA perfusion tracking dataset | This dataset was used to analyze the attachment of PDACs to the endothelium in Fig.7, SFig.7 and SFig8. | [Link to dataset](https://doi.org/10.5281/zenodo.13377961) |
| CD44 Blocking Antibody perfusion tracking dataset | This dataset was used to analyze the attachment of PDACs to the endothelium in Fig.7, SFig.7 and SFig8. | [Link to dataset](https://doi.org/10.5281/zenodo.13584215) |
| Hyaluronidase treatment perfusion tracking dataset | This dataset was used to analyze the attachment of PDACs to the endothelium in Fig.8. | [Link to dataset](https://doi.org/10.5281/zenodo.13627037) |


## [Structural Repetition Detector](https://github.com/HenriquesLab/SReD): multi-scale quantitative mapping of molecular complexes through microscopy

| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| SReD - Figure's data | This repository contains all the data related to the SReD paper | [View Dataset on Zenodo](https://zenodo.org/records/13764726) | [Mendes et al., 2024](https://www.biorxiv.org/content/10.1101/2024.09.16.613204v1.full) | 


## [PhotoFiTT](https://github.com/HenriquesLab/PhotoFiTT?tab=readme-ov-file): A Quantitative Framework for Assessing Phototoxicity in Live-Cell Microscopy Experiments

| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| PhotoFiTT: A Quantitative Framework for Assessing Phototoxicity in Live-Cell Microscopy Experiments | This repository contains all the data related to the study PhotoFiTT (Phototoxicity Fitness Time Trial) as well as example data for PhotoFiTT computational framework | [View Dataset on the BioImage Archive](https://www.ebi.ac.uk/biostudies/bioimages/studies/S-BIAD1269) | [Del Rosario et al., 2024](https://www.biorxiv.org/content/10.1101/2024.07.16.603046v2) | 


## [CellTracksColab](https://github.com/guijacquemet/CellTracksColab/tree/main) —A platform for compiling, analyzing, and exploring tracking data

| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| CellTracksColab - breast cancer cell dataset | Dataset used in the manuscript "CellTracksColab—A platform for compiling, analyzing, and exploring tracking data" | [View Dataset on Zenodo](https://zenodo.org/record/10539020) | [Gómez-de-Mariscal et al., 2024](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3002740) | 
| CellTracksColab - Filopodia dataset | Dataset used in the manuscript "CellTracksColab—A platform for compiling, analyzing, and exploring tracking data" | [View Dataset on Zenodo](https://zenodo.org/record/10539196) | [Gómez-de-Mariscal et al., 2024](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3002740) | 
| CellTracksColab - T cell dataset (full) | Dataset used in the manuscript "CellTracksColab—A platform for compiling, analyzing, and exploring tracking data" | [View Dataset on Zenodo](https://zenodo.org/record/10539720) | [Gómez-de-Mariscal et al., 2024](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3002740) | 

## [NanoPyx](https://github.com/HenriquesLab/NanoPyx): super-fast bioimage analysis powered by adaptive machine learning

| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- |
| NanoPyx - Figures' Data | NanoPyx - Figures' Data | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.8318395) | [Saraiva et al., 2023](https://www.biorxiv.org/content/10.1101/2023.08.13.553080v2)  |

## TLNRD1 is a CCM complex component and regulates endothelial barrier integrity
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| TLNRD1 figures | Raw microscopy images used to make the figures displayed in the article "TLNRD1 is a CCM complex component and regulates endothelial barrier integrity." | [View Dataset on Zenodo](https://zenodo.org/records/8377287) | [Ball et al., 2023](https://www.biorxiv.org/content/10.1101/2023.09.29.559344v1)  |

## High-fidelity 3D live-cell nanoscopy through data-driven enhanced super-resolution radial fluctuation

| Dataset Name | Description | Link | Reference |
| ------------ | ----------- | ---- | --------- |
| eSRRF - Supplementary Data | eSRRF datasets used in the manuscript | [View Dataset on Zenodo](https://zenodo.org/records/8325164) | [Laine et al., 2023](https://www.nature.com/articles/s41592-023-02057-w) |

## [Fast4DReg](https://github.com/CellMigrationLab/Fast4DReg): Fast registration of 4D microscopy datasets
| Dataset Name | Description | Link | Reference |
| ------------ | ----------- | ---- | --------- |
| Fast4DRegistration | Data used in the manuscript | [View Dataset on Zenodo](https://zenodo.org/records/6534570) | [Pylvänäinen et al., 2023](https://journals.biologists.com/jcs/article/136/4/jcs260728/287682/Fast4DReg-fast-registration-of-4D-microscopy)|
| Training dataset for Fast4DReg workshop | Fast4DReg workshop data | [View Dataset on Zenodo](https://zenodo.org/records/8347798) | [Pylvänäinen et al., 2023](https://journals.biologists.com/jcs/article/136/4/jcs260728/287682/Fast4DReg-fast-registration-of-4D-microscopy)|

## [TrackMate 7](https://imagej.net/plugins/trackmate/): integrating state-of-the-art segmentation algorithms into tracking pipelines

| Dataset Name | Description | Link | Reference |
| ------------ | ----------- | ---- | --------- |
| Tracking label images with TrackMate | Dataset used in a [tutorial](https://imagej.net/plugins/trackmate/trackmate-label-image-detector) on tracking label images with TrackMate. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5221424) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking with TrackMate using mask images of cell migration | Dataset used in a [tutorial](https://imagej.net/plugins/trackmate/trackmate-mask-detector) on tracking mask images with TrackMate. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5243127) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking cell migration with the TrackMate threshold detector | Dataset used in a [tutorial](https://imagej.net/plugins/trackmate/trackmate-thresholding-detector) on using the TrackMate threshold detector. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5220796) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| T cells migration followed with TrackMate | Dataset of T cells migrating on ICAM-1, tracked using StarDist in TrackMate. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5206119) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Segmenting cells in a spheroid in 3D using 2D StarDist within TrackMate | Dataset for segmenting cells in a 3D spheroid using 2D StarDist in TrackMate. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5220610) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking focal adhesions with TrackMate and Weka - tutorial dataset 1 | Dataset of MDA-mb-231 cells expressing GFP-paxillin for tracking focal adhesions. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5226842) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking focal adhesions with TrackMate and Weka - tutorial dataset 2 | Dataset of human dermal microvascular blood endothelial cells for tracking focal adhesions. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5978940) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking breast cancer cells migrating collectively with TrackMate-Cellpose | Dataset for tracking collective migration of breast cancer cells with TrackMate-Cellpose. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5864646) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Cancer cell migration followed with TrackMate | Dataset of migrating breast cancer cells for analysis with TrackMate. [tutorial](https://imagej.net/plugins/trackmate/trackmate-stardist). | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5206107) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Tracking Glioblastoma-astrocytoma cells with TrackMate-Cellpose | Dataset of Glioblastoma-astrocytoma U373 cells migrating on a polyacrylamide gel. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5863317) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Cell migration with ERK signalling | Movie following cells expressing ERK and a nuclei staining, tracked with TrackMate and later analyzed with MATLAB. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5205935) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |
| Quantitative comparison of tracking performance using TrackMate-Helper. | we used TrackMate-Helper to assess the performance of TrackMate on four datasets that cover a wide range of biological and imaging situations | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.6087729) | [Ershov et al., 2022](https://www.nature.com/articles/s41592-022-01507-1) |

## Cargo-specific recruitment in clathrin- and dynamin-independent endocytosis

| Dataset Name | Description | Link | Reference |
| ----------- | ---------- | ------- | --------- |
| Cancer cell migration followed with TrackMate | Stardist model and training dataset for automated tracking of MDA-MB-231 and BT20 cells | [View Dataset on Zenodo](https://zenodo.org/records/4812018) | [Moreno-Layseca et al., 2022](https://www.nature.com/articles/s41556-021-00767-x#Sec13) |


## Democratising deep learning for microscopy with [ZeroCostDL4Mic](https://github.com/HenriquesLab/ZeroCostDL4Mic)
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- |
| ZeroCostDL4Mic - Noise2Void (3D) example training and test dataset | A2780 ovarian carcinoma cells, transiently expressing Lifeact-RFP | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3713326) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - DeepSTORM training and example dataset | Experimental time-series dSTORM acquisition of Glial cells stained with phalloidin for actin | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3959089) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - Stardist example training and test dataset | Description not provided | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3713307) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - YoloV2 example training and test dataset | MDA-MB-231 cells migrating on cell-derived matrices generated by fibroblasts | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3941908) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - Label-free prediction (fnet) example training and test dataset | Hela labeled with TOM20 | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3748967) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - Noise2Void (2D) example training and test dataset | U-251 glioma cells, endogenously expressing paxillin-GFP | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3713315) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - CycleGAN example training and test dataset | Unpaired microscopy images (fluorescence) of microtubules (Spinning-disk and SRRF reconstructed images) | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3941884) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - CARE (3D) example training and test dataset | 3D paired microscopy images (fluorescence) of low and high signal-to-noise ratio | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.3713337) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - CARE (2D) example training and test dataset | Paired microscopy images (fluorescence) of low and high signal-to-noise ratio | [View Dataset on Zenodo](https://zenodo.org/records/3713330) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |
| ZeroCostDL4Mic - pix2pix example training and test dataset | Paired microscopy images (fluorescence) of lifeact-RFP and sir-DNA | [View Dataset on Zenodo](https://zenodo.org/records/3941889) | [von Chamier et al., 2021](https://www.nature.com/articles/s41467-021-22518-0) |

## Mapping the Localization of Proteins Within Filopodia Using [FiloMap](https://github.com/guijacquemet/FiloMAP)
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| FiloMap Test Dataset | Dataset for testing and validation in FiloMap, a tool that can be used to map the localization of proteins within filopodia from microscopy images. | [View Dataset on Zenodo](https://doi.org/10.5281/zenodo.5912949) | [Jacquemet et al., 2019](https://www.cell.com/current-biology/fulltext/S0960-9822(18)31552-5?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0960982218315525%3Fshowall%3Dtrue) and [Jacquemet et al., 2023](https://link.springer.com/protocol/10.1007/978-1-0716-2887-4_4) |

## Automated cell tracking using StarDist and TrackMate
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- |
Combining StarDist and TrackMate example 1 - Breast cancer cell dataset | Contains a StarDist example training dataset, a test dataset, and the StarDist model generated using ZeroCostDL4Mic | https://doi.org/10.5281/zenodo.4034976| [Fazeli et al., 2020](https://f1000research.com/articles/9-1279/v1)|
Combining StarDist and TrackMate example 2 - T cell dataset | Contains a StarDist example training dataset, a test dataset, and the StarDist model generated using ZeroCostDL4Mic | https://doi.org/10.5281/zenodo.4034929 | [Fazeli et al., 2020](https://f1000research.com/articles/9-1279/v1)|
Combining StarDist and TrackMate example 3 - Flow chamber dataset | Contains a StarDist example training dataset, a test dataset, and the StarDist model generated using ZeroCostDL4Mic | https://doi.org/10.5281/zenodo.4034939 | [Fazeli et al., 2020](https://f1000research.com/articles/9-1279/v1)|


## [FiloQuant](https://github.com/CellMigrationLab/FiloQuant) reveals increased filopodia density during breast cancer progression
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| S-JCBD-201704045 | Raw data from figures | [View Dataset](https://www.ebi.ac.uk/biostudies/jcb/studies/S-JCBD-201704045) | [Jacquemet et al., 2017](https://rupress.org/jcb/article/216/10/3387/38936/FiloQuant-reveals-increased-filopodia-density) |

## RCP-driven α5β1 recycling suppresses Rac and promotes RhoA activity via the RacGAP1–IQGAP1 complex
| Dataset Name | Description | Link | Reference | 
| ------------ | ----------- | ---- | --------- | 
| S-JCBD-201302041 | Raw data from figures | [View Dataset](https://www.ebi.ac.uk/biostudies/jcb/studies/S-JCBD-201302041) | [Jacquemet et al., 2013](https://rupress.org/jcb/article/216/10/3387/38936/FiloQuant-reveals-increased-filopodia-density) |

<!-- Add more rows as needed -->

