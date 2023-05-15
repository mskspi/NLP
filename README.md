# NLP

![NLP](img/Figure1.tif)

<img src="img/Figure1.tif" width="600">

For clustering of cell lines, the gene expression profiles for 915 cell lines were analyzed on the HPRD network. Invariant measures for individual nodes were then computed, and the Wasserstein distance (EMD) was computed between each pair of cell lines on the network. Lastly, hierarchical clustering was performed on the resultant Wasserstein distance matrix. For clustering of drugs, we obtained the cheminformatic features of 200 drugs, and built a data-driven network of cheminformatic features using the graphical LASSO. Similar to cell lines, hierarchical clustering was performed on the resultant Wasserstein distance matrix. 

<br />
<img src="img/Figure2.tif" width="600">

<br />
<img src="img/Figure3.tif" width="600">

<br />
<img src="img/Figure4.tif" width="600">

1. Model Building  
   - PathCNN.py  

2. GradCAM  
   - PathCNN_GradCAM_modeling.py: to generate a model for GradCAM (PathCNN_model.h5)
   - PathCNN_GradCAM.py: to generate GradCAM images and a resultant file (pathcnn_gradcam.csv)

3. Multi-omics data
   - GBM multi-omics data including mRNA expression, CNV, and DNA methylation were downloaded from the CBioPortal database.
   - Pathway information was downloaded from the KEGG database.
   - PCA was performed for each pathway in individual omics types.
   
   Five PCs in each omics type are in the following files:
   - PCA_EXP.xlsx, PCA_CNV.xlsx, PCA_MT.xlsx
   
   Clinival variables are in the following file:
   - Clinical.xlsx
