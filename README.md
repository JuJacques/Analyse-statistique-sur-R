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

## Test de dépendance entre deux variables aléatoires quantitatives
Question : y-a-t'il un lien l'âge du client et le montant total des avoirs dont il dispose sur tous les comptes ?

## Test de dépendance entre deux variables aléatoires qualitatives
Question : existe-il un lien entre la possession de la carte Visa-Premier et le code qualité du client ?

## Test de dépendance entre une variable aléatoire quantitative et une variable aléatoire qualitative
Question : le nombre de paiements par CB dépend-il du code qualité du client ?


