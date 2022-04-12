# Projet de détection d'infection pulmonaire

## Résumé / Abstract

Les techniques de vision par ordinateur peuvent être employées pour l’analyse d’images issues de capteurs
médicaux, par exemple pour l’aide au diagnostic et le suivi
de patient. L’objectif de ce projet est de proposer un
framework s’appuyant sur le deep learning pour identifier
automatiquement des infections pulmonaires à partir de
radiographies des poumons. Nous utiliserons une base de
données qui met à disposition des radiologies complètes de
patients (patient sain, patient souffrant de pneumonie,
patient souffrant de Covid-19). 


Environnement technique : Programmation en Python,
bibliothèques de vision par ordinateur (OpenCV, scikitimage), bibliothèque de deep learning Keras

Computer vision techniques can be used for the analysis of images from medical sensors, for example to
sensors, for example to help in diagnosis and patient monitoring.
of patients. The objective of this project is to propose a
framework based on deep learning to automatically identify
automatically identify lung infections from lung X-rays.
X-rays of the lungs. We will use a database that provides
database that provides complete radiologies of patients (healthy
patients (healthy patient, patient suffering from pneumonia
patient suffering from Covid-19). 


Technical environment: Programming in Python,
computer vision libraries (OpenCV, scikitimage), Keras deep learning library

## Organisation du repo

- "*pre_processing.ipynb*"

Le but de ce notebook est de réaliser l'ensemble des pre-processing utiles aux modèles d'apprentissages mis en place dans le notebook "model.ipynb". Afin de définir un couple modèle + pre-processing idéal, nous avons réalisé ici un total de 6 méthodes de pre-processing.

- "*model.ipynb*"

Le but de ce notebook est de réaliser de la K-fold cross validation sur les différents datasets que l'on a créé dans le notebook "pre_processing.ipynb". Les différentes méthodes de pre-processing y sont définies, ainsi nous conseillons de regarder le fichier en détail comprendre pour la différence entre chaque dataset. Ici les datasets sont utilisés avec les deux modèles suivants :
-- Un modèle RNN de convolution2D avec cellule GRU
-- Un modèle de convolution3D

