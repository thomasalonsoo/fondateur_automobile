# Les pilotes de formule 1


Ce projet vise à étudier l’évolution des parcours, des pratiques et des modes de sélection des pilotes de **Formule 1**, en les replaçant dans leurs contextes géographiques, sociaux et économiques, afin d’analyser la structure, les hiérarchies et les dynamiques du champ professionnel du pilotage automobile de haut niveau.    

###  Phase exploratoire

* [Problématique et questionnement](https://github.com/thomasalonsoo/fondateur_automobile/blob/main/Probl%C3%A9matique%20est%20questionnement)
* [Listes d'astronomes](Listes-d'astronomes.md)
* [Catalogue des informations](Catalogue-des-informations.md)

### Création de la base de données

*  [Modèle conceptuel](../MCD_to_database_example.png)
*  [Commentaire du modèle conceptuel](Modèle-conceptuel-commentaire.md)
*  [Modèle logique ou relationnel](Modèle-logique-ou-relationnel.md)

### Récupération et analyse de données existantes

* [Explorer DBpedia](DBpedia/DBpedia_explorer.md)
* [Importer les données de DBpedia](DBpedia/DBpedia_importer_dans_base_personnelle.md)
* [Visualiser les données de DBpedia](DBpedia/DBpedia_analyser_donnees_importees.md)



### Système d'information

[Table des matières](Table_des_pages.md) qui liste toutes les pages du wiki


### Analyse des données de Wikidata (notebooks Python)
* [Distribution des naissances dans le temps](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_distribution_naissances.ipynb)
* [Nationalités: production et codage des données](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_nationalite_production.ipynb)
* [Nationalités: analyse des données](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_nationalite_analyse.ipynb)
* [Genres: analyse des données](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_genre_analyse.ipynb)
* [Occupations: production et codage des données](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_occupations_production.ipynb)
* [Occupations: analyse des données](https://github.com/Sciences-historiques-numeriques/astronomers/blob/main/notebooks_jupyter/wikidata_exploration/wdt_occupations_analyse.ipynb)
 

### Résultats

* [Analyse de la distribution dans le temps et l'espace des naissances](results/birth_places_spatiotemporal_distribution.md)





# Pilotes de formule 1

Ce projet à pour but d'étudier la population des pilotes de formule 1

https://en.wikipedia.org/wiki/List_of_Formula_One_drivers

## Problématique

En adoptant une démarche exploratoire, il s’agit de proposer un modèle du champ des pilotes automobile (en s’appuyant sur les notions de champ et d’habitus de Pierre Bourdieu). L’objectif est de construire une représentation simplifiée de la structure du monde des pilotes de formule 1, c’est-à-dire des dynamiques sociales, économiques et culturelles qui le composent.
L’analyse portera sur les profils socio-démographiques des pilotes, leurs trajectoires et réseaux d’appartenance (parcours, partenaires, classes sociales, écuries, etc.), afin de mettre en évidence les formes de capital (économique, social, culturel, symbolique) mobilisées dans le parcours d'un pilote automobile. Par ailleurs, dans le cadre d'une approche prosopographique, nous collecterons systématiquement les caractéristiques des agents afin de mettre en évidence des profils biographiques et d'activité.

## Questions de recherche
- Existe-t-il une corrélation entre les origines sociales ou géographiques des pilotes et leur succès dans l'élite du pilotage automobile mondial? 
- Observe-t-on des spécificités générationnelles ou nationales dans les parcours (ex. : pilotes italiens, issus de familles riches, pilote de père en fils, etc.) ?
- Comment a évolué l’appartenance à des organisations ou institutions (centre d'entraienements, sponsoring, grands groupes industriels, etc.) au fil du temps ?
- Quels réseaux de relations (partenariats, sponsoring, collaborations techniques, filiales) structurent la carrière des pilotes et leurs évolutions ?
- Observe-t-on une homogénéisation progressive des trajectoires sociales, au profit de profils issus des classes supérieures ou de familles déjà intégrées au monde du sport automobile ?
- À partir de quand peut-on parler d’une standardisation des parcours vers la Formule 1 (académies, filières junior, contrats de développement) ?
- Comment évoluent les compétences valorisées (pilotage pur, travail technique, communication, image publique) et comment ces transformations influencent-elles les profils recrutés ?

## Aspects de l’information à collecter
- Origines géographiques et familiales des pilotes, profession et ressources des parents
- Formation sportive (karting, formules de promotion)
- Encadrement et apprentissages techniques (préparation physique, mentale, travail en simulateur)
- Expériences sportives successives avant et en Formule 1
- Appartenance à des institutions ou programmes (académies de pilotes, fédérations, écuries)
- Activités en dehors de la compétition (médias, sponsoring, engagements personnels)
- Résultats sportifs et productions professionnelles (palmarès, performances, rôles techniques)
- Relations, correspondances professionnelles et réseaux (managers, ingénieurs, sponsors, écuries)


## Catalogue-des-informations.md

Objets (avec leurs propriétés)
# Personne
- nom
- date de naissance
- ieu de naissance
- origine
- formation
- occupation
- publications

# Organisation
- nom
- type
- siège
- fondation

# Lieu
- nom
- type
- coordonnées géographiques

# Prix
- référence bibliographique
- année du prix
- lieu du prix

# Événement
- nom
- type (début de carrière, signature de contrat, accident, victoire majeure)
- date
- lieu
- personnes impliquées
- organisations associées

# Contrat / Engagement

- type (contrat sportif, sponsoring, programme junior)
- date de début
- date de fin
- organisation concernée
- personne concernée

# Relations entre objets

personne est née dans lieu
personne est fils de personne
personne est membre de organisation
personne est née dans lieu
personne est issue de personne
personne a été formée dans organisation
personne a travaillé pour organisation
personne est liée professionnellement à personne
personne participe à événement
organisation finance personne
organisation attribue prix
prix distingue personne
événement se déroule dans lieu
