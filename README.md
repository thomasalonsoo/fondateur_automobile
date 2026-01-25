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

# Objets (et leurs propriétés)
# Fondateur (Personne)
Nom
Date de naissance
Lieu de naissance
Nationalité
Origine sociale et familiale (milieu, profession des parents, statut économique) 
Formation (études techniques, ingénierie, commerce, autodidacte, etc.)
Expériences professionnelles (avant ou après la fondation de la marque)
Réseaux et collaborations (associés, mécènes, partenaires techniques investisseurs)
Publications / brevets / communications (liés à l’automobile ou à d’autres domaines)
Philosophie entrepreneuriale ou technique (vision de la marque, valeurs, innovations défendues)
Date et lieu de décès (si pertinent)

# Marque ou Entreprise (Organisation)
Nom de la marque / entreprise
Type d’entreprise (constructeur automobile, marque de luxe, constructeur de sport, etc.)
Siège social (ville, pays)
Date de fondation
Fondateur(s)
Forme juridique (société anonyme, entreprise familiale, etc.)
Secteur principal (véhicules particuliers, course, utilitaires, électriques, etc.)
Évolution de l’entreprise (fusion, rachat, succession, internationalisation, faillite, etc.)
Réseaux industriels (partenariats, sous-traitants, groupes, alliances techniques)

# Lieu
Nom du lieu (ville, région, pays)
Type de lieu (usine, atelier, siège, circuit automobile, école, etc.
Coordonnées géographiques
Période d’activité liée au fondateur ou à la marque 
Importance historique (lieu de création, d’innovation, de course, etc.)

# Innovation ou Modèle (Œuvre)
(équivalent de l’“œuvre” dans le champ scientifique, ici ce sont les créations techniques ou symboliques des fondateurs)
Nom du modèle ou innovation (ex. : Ford Model T, Ferrari 250 GTO, Tesla Roadster, etc.)
Type d’innovation (véhicule, moteur, châssis, technologie, design, brevet, etc.)
Année de création / présentation
Lieu de conception ou de production 
Marque / entreprise associée
Référence ou source documentaire (brevets, communiqués, expositions, presse)

# Relations entre objets
(adaptées pour refléter les dynamiques du monde automobile)
Fondateur est né dans → Lieu
Fondateur a étudié dans → Institution / école (Organisation)
Fondateur a fondé → Marque / entreprise (Organisation)
Fondateur a travaillé pour → Organisation
Fondateur a collaboré avec → Fondateur
Fondateur est inspiré par / mentor de → Fondateur
Fondateur est membre de → Organisation (club, école, groupe industriel, etc.)
Marque / entreprise a son siège à → Lieu
Marque / entreprise a été fondée dans → Lieu 
Marque / entreprise a produit → Innovation / modèle
Innovation / modèle a été conçue par → Fondateur ou Organisation 
Innovation / modèle a été présentée à → Lieu (salon, course, exposition)
Innovation / modèle a été publiée / brevetée en → Année / lieu

## Draw.io integration

This repository supports storing diagrams created with diagrams.net (Draw.io). Place `.drawio` source files under the `diagrams/` folder. A GitHub Actions workflow (`.github/workflows/drawio-export.yml`) automatically exports `.drawio` files to PNG and SVG in `diagrams/exports` on push. You can also trigger the workflow manually from the Actions tab on GitHub.

See `diagrams/README.md` for usage notes and conventions.
