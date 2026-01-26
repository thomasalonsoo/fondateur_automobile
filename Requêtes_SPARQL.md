Requêtes SPARQL

SELECT p.name, o.name, m. date_begin , m.date_end 
from membership m 
join person p on p.pk_person = m.fk_person 
JOIN organisation o on o.pk_organisation = m.fk_organisation; 

SELECT 
    o.name AS organisation,
    COUNT(m.fk_person) AS nombre_coureurs
FROM membership m
JOIN organisation o ON o.pk_organisation = m.fk_organisation
JOIN person p ON p.pk_person = m.fk_person
GROUP BY o.name
ORDER BY nombre_coureurs DESC;

