# Kaggle Competition SRAG

https://www.kaggle.com/competitions/ml-olympiad-ensure-healthy-lives/overview

O Ministério da Saúde (MS), por meio da Secretaria de Vigilância em Saúde (SVS), desenvolve a vigilância da Síndrome Respiratória Aguda Grave (SRAG) no Brasil, desde a pandemia de Influenza A(H1N1)pdm09. A partir disso, a vigilância de SRAG foi implantada na rede de vigilância de Influenza e outros vírus respiratórios, que anteriormente atuava exclusivamente com a vigilância sentinela de Síndrome Gripal (SG). O MS publicou o Guia de Vigilância Epidemiológica Emergência de Saúde Pública de Importância Nacional pela Doença pelo Coronavírus 2019 aonde estão disponíveis informações sobre definições de casos, critérios de confirmação e encerramento dos casos, dentre outros. https://opendatasus.saude.gov.br/

O objetivo da competição é de criar modelos para predizer qual o agente causador da síndrome respiratória aguda grave com base nos dados e sintomas dos pacientes.

**Table of contents**<a id='toc0_'></a>    
- [Get the Data and Preparing Features](#toc1_)    
    - [Classes Distribution](#toc1_1_1_)    
    - [High Null Values Columns](#toc1_1_2_)    
    - [Individual Columns](#toc1_1_3_)    
    - [Get Dummies (One-Hot-Encoding)](#toc1_1_4_)    
    - [Optimize df and drop negative perms from permutation rank features](#toc1_1_5_)    
- [Split and Preprocessing for Model](#toc2_)    
    - [Ordinal Encoder Strings](#toc2_1_1_)    
    - [Undersampling majority classes](#toc2_1_2_)    
    - [Missing Values](#toc2_1_3_)    
    - [Normalization](#toc2_1_4_)    
- [Models](#toc3_)    
    - [LightGBM](#toc3_1_1_)    
    - [Catboost](#toc3_1_2_)    
    - [XGboost](#toc3_1_3_)    
    - [Ranking Features (feature_importances and Permutation)](#toc3_1_4_)    
    - [Fine Tunning Model (optuna Lightgbm)](#toc3_1_5_)    
    - [Others Metrics (Gradient Boosting, Extra-Tree)](#toc3_1_6_)    
    - [Undersampling majority classes variations](#toc3_1_7_)    
- [Sample Submission and Stacking Ensemble](#toc4_)    
    - [Stack Ensemble Model](#toc4_1_1_)    
    - [Submission](#toc4_1_2_)    

<!-- vscode-jupyter-toc-config
	numbering=false
	anchor=true
	flat=false
	minLevel=1
	maxLevel=6
	/vscode-jupyter-toc-config -->
<!-- THIS CELL WILL BE REPLACED ON TOC UPDATE. DO NOT WRITE YOUR TEXT IN THIS CELL -->

