# Improved prediction of drug-induced liver injury literature using natural language processing and machine learning methods

**Challenge:** The Critical Assessment of Massive Data Analysis (CAMDA) 2022 in collaboration with the Intelligent Systems for Molecular Biology (ISMB) hosted the Literature AI for Drug Induced Liver Injury (DILI) challenge.  

## A pipeline of data analysis using natural language processing in conjunction with machine learning methods
<img src="img/Figure1.png" width="600">

## Internal and external validation strategy
<img src="img/Figure2.png" width="600">

## The top 10 most common words in (A) DILI-related and (B) unrelated literature
<img src="img/Figure3.png" width="600">

## The t-SNE visualization of the TF-IDF vectors obtained using (A) the title and abstract and (B) only the title of each publication
<img src="img/Figure4.png" width="600">


1. Data for modeling
   * DILIPositive.tsv: DILI-related literature (title + abstract)
   * DILINegative.tsv: DILI-unrelated literature (title + abstract)
2. External validaiton data
   * Requests to access data should be directed to CAMDA Challenge: http://camda.info/.
3. Code  
   * CAMDA_word_frequency.ipynb: To generate word frequecy and TSNE figures
   * CAMDA_word2vec+TFIDF.ipynb: Modeling and test using DILIPositive.tsv and DILINegative.tsv
   
