# README - Analyse des Sentiments avec LLM, BERT, RoBERTa, Spark NLP et LDA

## Description du projet
Ce projet se concentre sur l'analyse des sentiments à l'aide de modèles de langage de grande taille (LLM), en particulier BERT et RoBERTa, ainsi que d'outils de traitement du langage naturel tels que Spark NLP et LDA (Latent Dirichlet Allocation). L'objectif est de classer et d'analyser des textes afin de comprendre les émotions ou opinions véhiculées par les utilisateurs dans des documents textuels.

Les techniques employées dans ce projet permettent non seulement de détecter les sentiments, mais aussi d'extraire des sujets latents au sein des textes, offrant une vue d'ensemble des thématiques abordées par les utilisateurs.

## Méthodologie

### 1. **Prétraitement des données**
Les données textuelles sont nettoyées et préparées pour l'analyse. Cette étape inclut :
- **Nettoyage du texte** : suppression des caractères spéciaux, des stop words, des chiffres et ponctuations inutiles.
- **Tokenisation** : division des textes en mots ou tokens à l'aide de Spark NLP.
- **Stemming et lemmatisation** : réduction des mots à leurs racines, permettant une meilleure analyse sémantique.

### 2. **Modèles de Langage de Grande Taille (LLM)**
Des modèles pré-entraînés tels que **BERT** et **RoBERTa** sont utilisés pour l'analyse des sentiments. Ces modèles, basés sur des réseaux de neurones à attention (Transformers), permettent une meilleure compréhension du contexte dans les phrases et phrases complexes.

- **BERT** (Bidirectional Encoder Representations from Transformers) : utilisé pour une analyse fine des sentiments grâce à sa capacité à comprendre le contexte à partir des deux côtés du mot cible dans une phrase.
- **RoBERTa** : une version optimisée de BERT, plus performante dans certaines tâches de NLP, et utilisée pour obtenir des résultats précis dans la détection des sentiments.

### 3. **Analyse des sentiments avec Spark NLP**
Spark NLP est utilisé pour traiter de grandes quantités de texte rapidement et efficacement. En plus de la tokenisation et lemmatisation, Spark NLP facilite l'application de modèles de classification comme BERT et RoBERTa pour classer les sentiments des textes (positif, négatif, neutre).

### 4. **Latent Dirichlet Allocation (LDA) pour la modélisation des sujets**
En parallèle de l'analyse des sentiments, **LDA** est utilisé pour identifier les sujets dominants dans les documents textuels. LDA permet d'extraire les thèmes récurrents dans un ensemble de données textuelles, fournissant des informations sur les principaux centres d'intérêt ou préoccupations des utilisateurs.

### 5. **Visualisation des résultats**
Les résultats de l'analyse des sentiments et des sujets sont visualisés à l'aide d'outils comme **Matplotlib** et **Seaborn**. Les distributions des sentiments ainsi que les sujets identifiés par LDA sont représentés graphiquement pour une meilleure interprétation.

## Conclusion
Ce projet démontre l'efficacité de l'utilisation combinée des modèles LLM (BERT, RoBERTa) avec Spark NLP pour l'analyse des sentiments, ainsi que la capacité de LDA à extraire des sujets latents dans des corpus textuels. Les résultats obtenus permettent d'avoir une vue d'ensemble des opinions et thématiques présentes dans les documents étudiés, offrant ainsi des insights précieux pour des applications de marketing, de service client, ou de gestion de réputation.

## Requis pour l'exécution du projet
Pour exécuter ce projet, vous aurez besoin des outils et bibliothèques suivants :

- **Python 3.x**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Hugging Face Transformers** (pour BERT et RoBERTa)
- **Spark NLP**
- **Gensim** (pour LDA)
- **Jupyter Notebook**

## Instructions d'exécution

1. Clonez ce dépôt ou téléchargez les fichiers.
2. Installez les dépendances nécessaires via pip : `pip install -r requirements.txt`
3. Lancez le Jupyter Notebook : `jupyter notebook sentiment_analysis_with_llm.ipynb`
4. Suivez les étapes du notebook pour exécuter le projet et visualiser les résultats.

