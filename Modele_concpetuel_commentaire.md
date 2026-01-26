## Ce document contient le commentaire, avec exemples, du modèle conceptuel

## Person
Tout être humain.

Propriétés
Nom standard, date de naissance, lieu de naissance, nationalité, éventuellement origine sociale, éventuellement la date de mort. Il s'agit d'une classe objet (persistent item)

## Occupation
Un métier ou tout autre type d'occupation Il s'agit d'une classe objet (persistent item)

Propriétés
Nom standard, définition, date de début, date de fin.

Relations
Une relation réfléxive de spécialisation, termes plus génériques associés à des termes plus précis. Par exemple 'épicier' spécialise le terme de 'négociant'.

Pursuit
Le fait d'avoir telle occupation ou activité durant telle période Il s'agit d'une classe temporalité (temporal entity)

Exemple: "Schumacher était un pilote du grand prix de Monaco en 2006"

Relations
Une Pursuit peut comprend une et une seule personne, une et une seule occupation (ces deux relations sont nécessaires) et éventuellement on peut associer une (et une seule) organisation auprès de laquelle l'activité est exercée.

Si plusieurs organisation sont concernées par une activité, plusieurs individus de la classe Pursuit seront créées.

Tag
Un mot clé qui introduit un classement de recherche, généralement lié au questionnement.

Relations
Relation reflexive (d'un classe vers elle même) qui créer une taxonomie (i.e. une hiérarchie) de mots clés, les plus généraux étant les parents ou ancêtres des plus spécifiques.
