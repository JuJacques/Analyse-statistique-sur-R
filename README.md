# Analyses statistiques sur R

Cette page est dédiée à la formation doctorale transverse de l'Université de Lyon, destinée à tous les doctorants de l'UdL, quelque soit leur domaine de recherche.\
L'objectif de cette formation est d'introduire les principales notions d'inférence statistique (estimation, intervalle de confiance) ainsi que les tests statistiques (test de Student, test du Chi2, ANOVA, test de corrélation).\
La formation sera axée sur la pratique, à l'aide du logiciel R.

## Les données
Nous allons travailler avec le jeu de données `VisaPremier.txt`, donc le descriptif est du contenu est donné dans le fichier `VisaPremier.pdf`.
Ce jeux de données est un échantillon de client d'une banque. A partir de cet échantillon, nous allons chercher à tirer des informations sur l'ensemble des clients de cette banque.
Nous supposons pour cela que l'échantillon est représentatif de l'ensemble des clients de la banque.

### Exercice 1: prise en main
  - téléchargez le jeu de données sur votre ordinateur, dans un dossier dont vous choisirez le nom.
  - ouvrez Rstudio. Créer un fichier de script que vous enregistrerez, sous le nom `analyse-stat.R`, dans le même dossier que le fichier de données.
  - réglez le répertoire courant du terminal à l'endroit de votre fichier.
  - importer le fichier de données dans R.
  - réaliser une analyse exploratoire des données à l'aide de la commande `summary`, en vous aidant du fichier VisaPremier.pdf pour comprendre ce que signifie chaque variable.

## Traitement d'éventuelles données atypiques et des données manquantes

## Estimation ponctuelle et par intervalle de confiance
Nous allons travailler avec l'âge du client.

### Exercice 2: 
- faites la même chose avec l'ancienneté du client : représenter la distribution empirique de l'ancienneté ;
- estimer l'ancienneté moyenne pour l'ensemble de la population (ponctuellement et par intervalle de confiance de niveau 95%).
- Faites de même pour chaque code qualité des clients (de A à E) (représentation et estimation de la moyenne)

## Test de comparaison de deux sous-populations
Question : le nombre de paiements par CB est-il en moyenne différent pour les personnes qui possèdent la carte VP et celles qui ne la possèdent pas ?

### Exercice 3:
On souhaite tester l'effet d'un médicament censé réduire le taux de le cholesterol. On a mesuré le taux de cholesterol (g/l) chez 10 patients, avant la prise de ce médicament, et une semaine après l'avoir pris. Voici les taux obtenus :\
Avant 0.1  0.2 0.15 0.3 0.34 0.16 0.09 0.24 0.17 0.29\
Après 0.8  0.18 0.12 0.2 0.3 0.21 0.12 0.16 0.17 0.22\
Le médicament a-t-il un effet ?

## Test de dépendance entre deux variables aléatoires quantitatives
Question : y-a-t'il un lien l'âge du client et le montant total des avoirs dont il dispose sur tous les comptes ?

## Test de dépendance entre deux variables aléatoires qualitatives
Question : existe-il un lien entre la possession de la carte Visa-Premier et le code qualité du client ?

## Test de dépendance entre une variable aléatoire quantitative et une variable aléatoire qualitative
Question : le nombre de paiements par CB dépend-il du code qualité du client ?

## Applications 

### 1. Breast Tumors
Le jeu données 'breast.tumors.Rdata' contient le niveau d'expression de 1 000 gènes dans 47 échantillons chirurgicaux de tumeurs mammaires humaines provenant de 17 individus différents avant et après un traitement de chimiothérapie. Quels sont les gènes dont le niveau d'expression est impacté par la chimiothérapie ?

### 2. Taux de fer
On s'intéresse au taux de fer présent dans le foie et le régime à suivre pour mieux contrôler ce taux. On souhaite comparer l'effet des 5 régimes. Il s'agit d'une étude sur des souris. Le plan d'expérience consiste à assigner de manière aléatoire 9 souris pour chaque régime (on considère que la durée du régime est suffisamment grande pour qu'elle efface les éventuelles différences entre les souris avant le régime). Les résultats sont disponibles dans le fichier 'Taux de fer.txt'.\
Y-a-t'il une différence entre les souris ?
