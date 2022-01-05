# TLN-TP-SA-Analyse-de-sentiments 
Analyse de polarité de mots dans des commentaires avec SVM

# Objectif du projet
Le projet a pour but de nous apprendre à créer un modèle capable de prédire, de la manière la plus optimale possible, la polarité d'un mot dans une phrase. la polarité du mot peut être Positive, Négative ou Neutre. 

# Contenu du projet
## Les données
### Fichiers
Dans le répertoire git se trouve 2 fichiers .ipynb (fichiers de notebook de Collab). Un fichier est pour la partie "Restaurants" et le second pour la partie "Laptop".
De plus vous trouverez, l'ensemble des xml nécessaires à la bonne exécutions des notebook. (fichiers de train et tests)

### Variable à prédire
Ici la variable à prédire est la polarité (polarity) --> Polarité du terme auquelle elle est associée

### Caractéristiques utilisées 
Dans notre cas les caractéristiques les plus importantes à utiliser sont :
* term : le terme à étudier (dont on doit prédire la polarité)
* text : la phrase complète dans laquelle se trouve le terme
* senti word : les mots retenus connus de sentiword pour l'analyse
* score by word : le score pour chaque mot connu de sentiword (le score peut etre vide, par exempe "le" n'a pas de polarité)
* pos tag : les posTag obtenu à partir de la tokenization (CC, CD, DT, EX, FW ...) 

## Les résultats
Je n'affiche dans ce README que les résultats obtenus avec un kernel polynomial car d'après les tests faits dans le notebook se sont les meilleurs résultats

### Restaurants
![image](https://user-images.githubusercontent.com/28843048/148211157-c7d3e610-fb6d-4b60-ac6b-2b728ef216ce.png)

### Laptop
![image](https://user-images.githubusercontent.com/28843048/148211113-30f9f5ac-617a-479e-b112-1ffd6ee1f06b.png)
