# TP_ML_IDL
TP du cours d'apprentissage automatique du master 2 science du langage, parcours IDL
Université Grenoble Alpes - Année universitaire 2022-2023

1. **TP CNN : Classification d'expressions faciales par les Réseaux de Neurones Convolutifs**
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11-4X3fYpr0X1EcVFrYVdZuIs4JXdGpoP?usp=sharing)

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


