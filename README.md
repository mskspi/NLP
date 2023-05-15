# Improved prediction of drug-induced liver injury literature using natural language processing and machine learning methods

**Challenge:** The Critical Assessment of Massive Data Analysis (CAMDA) 2022 in collaboration with the Intelligent Systems for Molecular Biology (ISMB) hosted the Literature AI for Drug Induced Liver Injury (DILI) challenge. A curated dataset, consisting of 277,016 DILI annotated papers, was downloaded from the CAMDA website. All the papers were labeled as DILI-related (referred to as “positive samples”) or irrelevant to DILI (referred to as “negative samples”) by a panel of DILI experts. For the CAMDA challenge, the labels for 7,177 DILI-related papers and 7,026 DILI-unrelated papers were released while the labels for the remaining papers (N=262,813) were masked for model assessment and were split into three test sets and four validation sets. In this study, 14,203 papers with positive or negative labels were used for model building. For each paper, the title and abstract were provided and concatenated to be used in modeling. 

<br />
<img src="img/Figure1.png" width="600">
Figure 1. A pipeline of data analysis using natural language processing in conjunction with machine learning methods.  
<br />
<br />
<img src="img/Figure2.png" width="600">
Figure 2. Internal and external validation strategy. 
<br />
<br />
<img src="img/Figure3.png" width="600">
Figure 3. The top 10 most common words in (A) DILI-related and (B) unrelated literature.
<br />
<br />
<img src="img/Figure4.png" width="600">
Figure 4. The t-SNE visualization of the TF-IDF vectors obtained using (A) the title and abstract and (B) only the title of each publication.
<br />
<br />
1. Model Building  
   - PathCNN.py  
   -
2. GradCAM  
   - PathCNN_GradCAM_modeling.py: to generate a model for GradCAM (PathCNN_model.h5)
   - PathCNN_GradCAM.py: to generate GradCAM images and a resultant file (pathcnn_gradcam.csv)
   
3. Data
   - All data were made available to participants by the CAMDA challenge organizers. Requests to access data should be directed to CAMDA Challenge: http://camda.info/.
