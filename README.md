# TP_ML_IDL
TP du cours d'apprentissage automatique du master 2 science du langage, parcours IDL

Université Grenoble Alpes - Année universitaire 2022-2023

## **1. TP CNN : Classification d'expressions faciales par les Réseaux de Neurones Convolutifs** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11-4X3fYpr0X1EcVFrYVdZuIs4JXdGpoP?usp=sharing)

Dans ce TP, vous allez entraîner un modèle CNN (ConvNet) pour classifier les expressions faciales. 

Les entrées du modèles sont des images de visages en niveaux de gris de 48 x 48 pixels étiquettes avec sept classes : colère, dégoût, peur, joie, tristesse, surprise, neutre. 

Les objectifs de ce TP sont de :
* Manipuler un jeu de données d'images afin de le préparer à être traiter par un réseau de neurones. 
* Définir et implanter une architecture CNN pour réaliser un classifier d'images
* Créer une boucle d'entraînement en complétant les fonctions *train* et *evaluation*.
* Entraîner un modèle et analyser les performances 

L'ensemble du TP sera effectuer avec la bibliothèque d'apprentissage profond PyTorch. 

Référence :
1. [Tutorials > Deep Learning with PyTorch: A 60 Minute Blitz > Training a Classifier](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)
2. Corpus disponible sur kaggle: [Face expression recognition dataset](https://www.kaggle.com/datasets/jonathanoheix/face-expression-recognition-dataset) 
3. Explications sur les différentes couches : [Comprendre les Réseaux de Neurones Convolutifs (CNN)](https://yannicksergeobam.medium.com/comprendre-les-r%C3%A9seaux-de-neurones-convolutifs-cnn-d5f14d963714)

## **2. TP NMT : Méthodes de la traduction automatique neuronale**
### TP1 : Modèle de traduction simple (deux RNNs, sans méchanisme d'attention) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1Dgs23InXNQhtaOnkw42Oa53i768YOGqb/view?usp=sharing)

Dans ce TP du cours `Modèles avancés d'apprentissage automatique`, vous allez vous initier aux méthodes de traduction automatique neuronales notamment aux architecture Encodeur-Décodeur. 

Dans ce premier TP, l'objectif est d'étudier et d'entraîner un modèle Encodeur-Décodeur simple en utilisant deux RNNs. La tâche sera de traduire de l'anglais vers le français. Cette tâche de traduction automatique sera réalisée à l'aide d'un modèle de séquence à séquence [Sequence to Sequence Learning with Neural Networks](https://arxiv.org/abs/1409.3215), dans lequel deux réseaux neuronaux récurrents travaillent de concert pour transformer une séquence de mots d'entrée en une autre séquence de mots de sortie. La qualité de la traduction sera évaluée en utilisant la métrique BLEU. 

Pour ce faire, vous travaillerez sur ce *Jupyter Notebook* qui utilisera un dossier `pyfiles` contenant trois fichiers python (`py`), qui traitent la préparation de données et la mise en oeuvre des modèles. Vous n'aurez pas à modifier ces fichiers. 

Vous utiliserez les outils suivants:
1. [PyTorch](https://pytorch.org/docs/stable/index.html) : une bibliothèque Python *open-source* pour l'apprentissage automatique
2. Google Colab, qui héberge ce *Jupyter Notebook*. 

### TP2 : Modèle de traduction simple (deux RNNs, avec méchanisme d'attention) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1U8G0tGuPSPxDOIGU-TgguKXVKWDifD6m/view?usp=sharing)

Ce TP du cours Modèles avancés d'apprentissage automatique, est la suite du TP de traduction automatique neuronale utilisant une architecture Encodeur-Décodeur.

Dans ce deuxième TP, l'objectif est d'étudier le mécanisme d'attention ajouté au modèle Encodeur-Décodeur. Toute la première partie sur le traitement du corpus reste similaire au TP précédent. Les modifications apportées se trouvant à partir de la définition du modèle.

[TP2_NMT_QA.docx](https://cloud.univ-grenoble-alpes.fr/s/yZeLsz7PZqDeQBE)

### TP3 : Modèle de traduction composé de transformer [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1BpwZ2fNaUul65yCNbTdPu1zIA5I8SK9Z?usp=sharing)

Ce TP du cours Modèles avancés d'apprentissage automatique, est la suite du TP de traduction automatique neuronale utilisant une architecture Encodeur-Décodeur sans et avec le mécanisme d'attention.

L'architecture transformer (cf. l'article Attention Is All You Need) est maintenant l'état de l'art de la traduction automatique neuronale. L'encodeur utilise un mécanisme de self-attention sur les couches d'entrée tandis que le décodeur combine la self-attention et l'attention sur l'encodeur. Contrairement au RNN, aucune recurrence n'est utilisée. De ce fait un modèle transformer est plus rapide à apprendre.
