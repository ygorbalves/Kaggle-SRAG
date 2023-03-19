# Kaggle Competition SRAG

https://www.kaggle.com/competitions/ml-olympiad-ensure-healthy-lives/overview

O Ministério da Saúde (MS), por meio da Secretaria de Vigilância em Saúde (SVS), desenvolve a vigilância da Síndrome Respiratória Aguda Grave (SRAG) no Brasil, desde a pandemia de Influenza A(H1N1)pdm09. A partir disso, a vigilância de SRAG foi implantada na rede de vigilância de Influenza e outros vírus respiratórios, que anteriormente atuava exclusivamente com a vigilância sentinela de Síndrome Gripal (SG). O MS publicou o Guia de Vigilância Epidemiológica Emergência de Saúde Pública de Importância Nacional pela Doença pelo Coronavírus 2019 aonde estão disponíveis informações sobre definições de casos, critérios de confirmação e encerramento dos casos, dentre outros. https://opendatasus.saude.gov.br/

O objetivo da competição é de criar modelos para predizer qual o agente causador da síndrome respiratória aguda grave com base nos dados e sintomas dos pacientes.

**Table of contents** 
- Get the Data and Preparing Features 
    - Classes Distribution  
    - High Null Values Columns   
    - Individual Columns 
    - Get Dummies (One-Hot-Encoding) 
    - Optimize df and drop negative perms from permutation rank features 
- Split and Preprocessing for Model  
    - Ordinal Encoder Strings   
    - Undersampling majority classes    
    - Missing Values    
    - Normalization 
- Models   
    - LightGBM    
    - Catboost 
    - XGboost   
    - Ranking Features (feature_importances and Permutation)   
    - Fine Tunning Model (optuna Lightgbm)
    - Others Metrics (Gradient Boosting, Extra-Tree)   
    - Undersampling majority classes variations   
- Sample Submission and Stacking Ensemble   
    - Stack Ensemble Model  
    - Submission 

<!-- vscode-jupyter-toc-config
	numbering=false
	anchor=true
	flat=false
	minLevel=1
	maxLevel=6
	/vscode-jupyter-toc-config -->
<!-- THIS CELL WILL BE REPLACED ON TOC UPDATE. DO NOT WRITE YOUR TEXT IN THIS CELL -->

