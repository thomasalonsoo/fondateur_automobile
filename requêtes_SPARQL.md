## Voici ici les recherches que j'ai réussi à réaliser pour https://dbpedia.org/sparql: 


## Compte le nombre de pilotes: 

PREFIX dbo: <http://dbpedia.org/ontology/>

SELECT (COUNT(*) AS ?effectif)
WHERE {
  ?pilot a dbo:FormulaOneRacer .
}


## Donne le nombre de pilotes par tranche d'âge de 20 ans à partir de 1900, donc de 1900 à 1920, de 1920 à 1940, etc. 

PREFIX dbo: <http://dbpedia.org/ontology/>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>

SELECT ?tranche (COUNT(DISTINCT ?driver) AS ?nb_pilotes)
WHERE {
  ?driver a dbo:FormulaOneRacer ;
          dbo:birthDate ?birthDate .

  BIND(year(?birthDate) AS ?y)
  BIND( (xsd:integer(floor(?y/20)*20)) AS ?start )
  BIND( CONCAT(STR(?start), "-", STR(?start + 20)) AS ?tranche )

  FILTER(?y >= 1900 && ?y < 2020)
}
GROUP BY ?tranche
ORDER BY ASC(?tranche)


## Voici une recherche qui m'a pris plus d'une heure à réaliser (avec de l'aide d'un ami)... elle donne le nombre de pilotes pour les 5 pays suivants (Italie, France, Allemagne, Grande Bretagne, USA) : 
    
    PREFIX dbo: <http://dbpedia.org/ontology/>
PREFIX dbp: <http://dbpedia.org/property/>
PREFIX dbr: <http://dbpedia.org/resource/>

SELECT ?pays (COUNT(DISTINCT ?driver) AS ?nb_pilotes)
WHERE {
  ?driver a dbo:FormulaOneRacer .

  {
    # Cas 1 & 2 : dbo:nationality en ressource (pays ou adjectif)
    VALUES (?nat ?pays) {
      (dbr:France          "France")
      (dbr:French          "France")
      (dbr:Italy           "Italy")
      (dbr:Italian         "Italy")
      (dbr:Germany         "Germany")
      (dbr:German          "Germany")
      (dbr:United_Kingdom  "United Kingdom")
      (dbr:British         "United Kingdom")
      (dbr:United_States   "United States")
      (dbr:American        "United States")
    }
    ?driver dbo:nationality ?nat .
  }
  UNION
  {
    # Cas 3 : dbp:nationality en texte (infobox)
    ?driver dbp:nationality ?natTxt .
    BIND(STR(?natTxt) AS ?n)

    BIND(
      IF(CONTAINS(LCASE(?n), "french"), "France",
      IF(CONTAINS(LCASE(?n), "italian"), "Italy",
      IF(CONTAINS(LCASE(?n), "german"), "Germany",
      IF(CONTAINS(LCASE(?n), "british") || CONTAINS(LCASE(?n), "uk") || CONTAINS(LCASE(?n), "united kingdom"), "United Kingdom",
      IF(CONTAINS(LCASE(?n), "american") || CONTAINS(LCASE(?n), "united states") || CONTAINS(LCASE(?n), "usa"), "United States",
      ""))))) AS ?pays
    )

    FILTER(?pays != "")
  }
}
GROUP BY ?pays
ORDER BY DESC(?nb_pilotes)
 
