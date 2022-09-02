# Requêtes SPARQL
## Pour créer l'index spatial pour utiliser GeoSPARQL :
```sparql
PREFIX geosparql: <http://www.ontotext.com/plugins/geosparql#>

INSERT DATA {
  [] geosparql:enabled "true" .
}
```
## Exemples de requêtes

Peut-on pratiquer la Grande Passe de nuit ?
Pour avoir les informations liées à la Grande Passe de nuit :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX tit: <http://data.shom.fr/id/codes/nav/typedindicationtemporelle/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
SELECT DISTINCT ?propriete ?info ?temporalite
WHERE {
?s rdf:type nav:Information.
?s nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet rdfs:label "Grande Passe"@fr.
?s nav:aPourTemporalite ?temporalite.
?s ?propriete ?info.
}
```

Y a-t-il des interdictions au sein du parc naturel marin d’Iroise ?
Pour avoir toutes les informations concernant toutes les interdictions dans le parc naturel marin d'Iroise :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
SELECT DISTINCT ?propriete ?info ?info2
WHERE {
?ent rdf:type nav:Interdiction.
?ent nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet rdfs:label "parc naturel marin d'Iroise"@fr.
?ent ?propriete ?info
    OPTIONAL {?info rdfs:label ?info2}
}
```

Quand peut-on mouiller dans la zone 6032 ? (ent:6032 parce qu'il s'agit d'une entité non-nommé)
Pour avoir toutes les consignes à propos de mouiller dans la zone 6032 :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
SELECT ?propriete ?info
WHERE {
?ent nav:aPourAction tac:Mouillage.
?ent nav:aPourLieuDEffet ent:6032.
?ent ?propriete ?info
}
```

Où est située la zone interdire de la centrale de Gravelines ?
Pour avoir toutes les informations sur la zone interdite de la centrale de Gravelines :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
SELECT DISTINCT ?propriete ?info
WHERE {
?ent rdfs:label "Zone interdite de la centrale de Gravelines".
?ent nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet ?propriete ?info.
}
```

Quel arrêté est à l'origine de la Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
SELECT ?arrêté
WHERE {
?ent nav:estImposeePar ?règlement.
?ent nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet rdfs:label "Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque"@fr.
?règlement nav:aPourArrete ?arrêté
}
```

Comment puis-je contacter le Bureau du port à Saint-Valéry-sur-Somme ?
Pour avoir tous les moyens de contacter le Bureau du port à Saint-Valéry-sur-Somme et les informations complémentaires :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
SELECT ?propriete ?info
WHERE {
?ent rdf:type nav:Renseignement.
?ent nav:aPourContact ?contact.
    FILTER (regex(str(?contact), "Bureau du port" ))
?ent nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet rdfs:label "Saint-Valéry-sur-Somme"@fr.
?ent ?propriete ?info
}
```

Qui peut-on contacter à Courseulles-sur-Mer ? Quels sont leurs numéros de téléphone ? Y a-t-il des horaires associées aux numéros de téléphone ?
Pour avoir tous les contacts à Courseulles-sur-Mer :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
SELECT ?propriete ?info
WHERE {
?ent rdf:type nav:Renseignement.
?ent nav:aPourContact ?contact.
?ent nav:aPourLieuDEffet ?lieuDEffet.
?lieuDEffet rdfs:label "Courseulles-sur-Mer"@fr.
?ent ?propriete ?info
}
```

Est-ce qu'il est possible d'accoster la balise « Jet d’Amont » ?
Pour avoir des consignes concernant la balise :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg: <http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
SELECT DISTINCT *
WHERE {
?ent nav:aPourEntiteImpliquee/rdfs:label "Jet d’Amont"@fr.
?ent a nav:ConsigneDeNavigation.
?ent nav:aPourAction tac:Accostage.
    ?ent ?propriete ?objet
}
```

Pour trouver les 5 entités les plus proches à une autre entité donnée (ent:6005) :
```sparql
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX uom: <http://www.opengis.net/def/uom/OGC/1.0/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?f ?fL ?fGeom
WHERE {
    ent:6005 geom:hasGeometry ?cGeom .
    ?cGeom gsp:asWKT ?cWKT .
    ?f geom:hasGeometry ?fGeom .
    ?fGeom gsp:asWKT ?fWKT .
    FILTER (?fGeom != ?cGeom)
    ?f rdfs:label ?fL
}
ORDER BY ASC(geof:distance(?cWKT, ?fWKT, uom:metre))
LIMIT 5
```

Pour donner le linestring le plus court qui relie deux points en WKT :
```sparql
PREFIX xsd:  <http://www.w3.org/2001/XMLSchema#>
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX ext: <http://rdf.useekm.com/ext#>
PREFIX uom: <http://www.opengis.net/def/uom/OGC/1.0/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

SELECT ?line
WHERE {
     ent:6005 geom:hasGeometry ?g1.
     ?g1 gsp:asWKT ?lit1.
    ent:6004 geom:hasGeometry ?g2.
     ?g2 gsp:asWKT ?lit2.
BIND(ext:shortestLine(?lit1, ?lit2) as ?line).
}
```

Pour créer une nouvelle entité (ent:7001) qui est le linestring le plus court qui relie deux entités données :
```sparql
PREFIX xsd:  <http://www.w3.org/2001/XMLSchema#>
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX ext: <http://rdf.useekm.com/ext#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>

CONSTRUCT {ent:7001 a geom:LineString.
    ent:7001 gsp:asWKT ?line}
WHERE {
     ent:6005 geom:hasGeometry ?g1.
     ?g1 gsp:asWKT ?lit1.
    ent:6004 geom:hasGeometry ?g2.
     ?g2 gsp:asWKT ?lit2.
BIND(ext:shortestLine(?lit1, ?lit2) as ?line).
}
```

Pour trouver tous les alignements dans la base et donner le linestring en WKT entre les deux repères à chaque fois :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX ext: <http://rdf.useekm.com/ext#>

SELECT DISTINCT ?line ?nature1 ?label1 ?nature2 ?label2
WHERE {
?ent a nav:Alignement.
?ent nav:aPourRepere ?nb.
    ?nb ?relation1 ?entite1.
    OPTIONAL {?entite1 rdfs:label ?label1; nav:aPourNature ?nature1}
    FILTER (strstarts(str(?relation1), str(rdf:_1)))
    ?entite1 geom:hasGeometry ?g1.
?ent nav:aPourRepere ?nb2.
    ?nb2 ?relation2 ?entite2.
    OPTIONAL {?entite2 rdfs:label ?label2}
    OPTIONAL {?entite2 nav:aPourNature ?nature2}
    FILTER (strstarts(str(?relation2), str(rdf:_2)))
    ?entite2 geom:hasGeometry ?g2.
?g1 gsp:asWKT ?lit1.
?g2 gsp:asWKT ?lit2.
BIND(ext:shortestLine(?lit1, ?lit2) as ?line).
}
```

Pour calculer tous les linestrings entre chaque paire de points qui constituent un alignement, les associer un uri et créer le graphe correspondant. Donne le linestring en WKT WSG84.
```sparql
PREFIX xsd:  <http://www.w3.org/2001/XMLSchema#>
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX ext: <http://rdf.useekm.com/ext#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>

CONSTRUCT {?uri a geom:LineString; gsp:asWKT ?line.
			?entGeo geom:hasGeometry ?uri}
WHERE {
     BIND (IRI(CONCAT("http://data.shom.fr/id/codes/nav/geometries/", strUUID())) AS ?uri)
?entGeo a nav:Alignement.
?entGeo nav:aPourRepere ?nb.
    ?nb ?relation1 ?entite1.
    FILTER (strstarts(str(?relation1), str(rdf:_1)))
    ?entite1 geom:hasGeometry ?g1.
?entGeo nav:aPourRepere ?nb.
    ?nb ?relation2 ?entite2.
    FILTER (strstarts(str(?relation2), str(rdf:_2)))
    ?entite2 geom:hasGeometry ?g2.
?g1 gsp:asWKT ?lit1.
?g2 gsp:asWKT ?lit2.
BIND(ext:shortestLine(?lit1, ?lit2) as ?line).
}
```

Quels sont les caractéristiques du phare de l'Île de Batz ?
Pour avoir les caractéristiques physiques et les caractéristiques géographiques (les relations spatiales) du phare de l'Ile de Batz :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT DISTINCT ?propriete1 ?info1 ?propriete2 ?info2 ?propriete3 ?info3 ?unité
WHERE {
?ent1 nav:aPourNature teg:Phare.
?ent1 nav:estUnElementDe ?ent2.
?ent2 rdfs:label "île de Batz"@fr.
    OPTIONAL {?ent1 nav:aPourCaracteristique ?info1.
    ?ent1 ?propriete1 ?info1}
    OPTIONAL {?ent1 nav:aUneRelationSpatialeAvec ?info2.
    ?ent1 ?propriete2 ?info2}
    OPTIONAL {?ent1 nav:aPourDimension ?info3.
        <<?ent1 ?propriete3 ?info3>> qudt:Unit ?unité.}
}
```

Quelle est la profondeur du Canal de l’Île de Batz ?
Pour avoir toutes les mesures de profondeur du Canal de l'Ile de Batz :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?aPourProfondeurEau ?valeur ?unit
WHERE {
?entité rdfs:label "Canal de l'Île de Batz"@fr.
<<?entité ?aPourProfondeurEau ?valeur>> qudt:Unit ?unit.
}
```

Où peut-on mouiller dans le chenal 4011 ?
Pour avoir toutes les lieux de stationnement dans le chenal :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT DISTINCT ?propriete ?info
WHERE {
?ent nav:estSitueDans ent:4011.
?ent nav:aPourNature ?lieuDeStationnement.
?lieuDeStationnement a nav:TypeDeLieuDeStationnement.
?ent ?propriete ?info
}
```

Quelles sont les coordonnées géographiques de Porz Kernok ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT DISTINCT ?typeDeCoordonneeGeographique ?coordonnees
WHERE {
?entité rdfs:label ?nom.
        FILTER (regex(str(?nom), "Porz Kernok" ))
?entité nav:aPourCoordonneesGeographiques ?coordonnees.
?entité ?typeDeCoordonneeGeographique ?coordonnees
}
```

Où se trouve le clocher de Roscoff ?
Pour avoir les coordonnées géographiques et les relations spatiales autour du clocher de Roscoff :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
SELECT ?typeDeCoordonneeGeographique ?coordonnees ?typeDeRelationSpatiale ?nom ?wkt
WHERE {
?entité rdfs:label "clocher de Roscoff"@fr.
    OPTIONAL {?entité nav:aPourCoordonneesGeographiques ?coordonnees.
        ?entité ?typeDeCoordonneeGeographique ?coordonnees}
    OPTIONAL {?entité nav:aUneRelationSpatialeAvec ?autreEntité.
        ?entité ?typeDeRelationSpatiale ?autreEntité.
        ?autreEntité rdfs:label ?nom}
    OPTIONAL {?entité geom:hasGeometry ?geom.
    ?geom gsp:asWKT ?wkt}
}
```

Comment peut-on stationner dans le port de Moguériec ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?nom
WHERE {
?entité rdfs:label "Moguériec"@fr.
?entité nav:aPourNature teg:Port.
?entité nav:aPourElement ?lieuDeStationnement.
?lieuDeStationnement nav:aPourNature ?nom.
}
```

Est-ce que Porz Guen est protégé ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?typeDeRelationSpatiale ?typeDeProtection
WHERE {
?entité rdfs:label "échouage de Porz Guen"@fr.
?entité nav:estProtegePar ?autreEntité.
?autreEntité nav:aPourNature ?typeDeProtection.
?entité nav:aUneRelationSpatialeAvec ?autreEntité.
?entité ?typeDeRelationSpatiale ?autreEntité
}
```

Quelles sont les dimensions du chenal de La Malouine ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?typeDeDimension ?dimension ?unit
WHERE {
?entité rdfs:label "chenal de La Malouine"@fr.
?entité nav:aPourDimension ?dimension.
<<?entité ?typeDeDimension ?dimension>> qudt:Unit ?unit.
}
```

Où se trouve le mouillage de Karreg Du ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT DISTINCT ?entité ?relation ?nom
WHERE {
?entité rdfs:label "Karreg Du"@fr.
?entité nav:aUneRelationSpatialeAvec ?selection.
?selection ?label ?autreEntité.
    FILTER (strstarts(str(?label), str(rdf:_)))
?autreEntité rdfs:label ?nom.
?entité ?relation ?selection
}
```

Comment sont les rochers Roustel et Platte marquées ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?marqueRocherRoustel ?typeDeCaractéristique ?caractéristique
WHERE {
?entité rdfs:label "rocher Roustel"@fr.
?entité nav:estMarquePar ?marqueRocherRoustel.
?marqueRocherRoustel nav:aPourCaracteristique ?caractéristique.
?marqueRocherRoustel ?typeDeCaractéristique ?caractéristique
}

PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX unit: <http://qudt.org/2.1/vocab/unit/>
SELECT ?marqueRocherPlatte ?typeDeCaractéristique ?caractéristique
WHERE {
?entité rdfs:label "rocher Platte"@fr.
?entité nav:estMarquePar ?marqueRocherPlatte.
?marqueRocherRoustel nav:aPourCaracteristique ?caractéristique.
?marqueRocherPlatte ?typeDeCaractéristique ?caractéristique
}
```

Pour trouver tous les amers qui se trouvent sur l'Île de Batz :
```sparql
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geof: <http://www.opengis.net/def/function/geosparql/>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>

SELECT ?amer ?typeDAmer ?labelAmer
WHERE {
    ent:4001 geom:hasGeometry ?GeomIdB.
    ?GeomIdB gsp:asWKT ?WKTIdB.
    ?amer nav:aPourNature ?typeDAmer.
    ?typeDAmer a nav:TypeDAmer.
    ?amer geom:hasGeometry ?GeomAmer.
    ?GeomAmer gsp:asWKT ?WKTAmer.
    OPTIONAL {?amer rdfs:label ?labelAmer}.
    FILTER (geof:sfContains(?WKTIdB, ?WKTAmer) && !sameTerm(?GeomIdB, ?GeomAmer)).
}
```
OU
```sparql
PREFIX gsp: <http://www.opengis.net/ont/geosparql#>
PREFIX geom: <http://data.ign.fr/def/geometrie#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX ext: <http://rdf.useekm.com/ext#>
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>

SELECT ?amer ?typeDAmer ?labelAmer
WHERE {
    ent:4001 geom:hasGeometry ?GeomIdB.
    ?GeomIdB gsp:asWKT ?WKTIdB.
 	?amer nav:aPourNature ?typeDAmer.
    ?typeDAmer a nav:TypeDAmer.
    ?amer geom:hasGeometry ?GeomAmer.
    ?GeomAmer gsp:asWKT ?WKTAmer.
    OPTIONAL {?amer rdfs:label ?labelAmer}.
    FILTER (ext:containsProperly(?WKTIdB, ?WKTAmer) && !sameTerm(?GeomIdB, ?GeomAmer)).
}
```

Quels sont les phénomènes météorologiques ou océanographiques qui affectent la navigation dans le milieu du chenal 5001 ?
Pour avoir toutes les informations concernant les phénomènes météorologiques et océanographiques au milieu du chenal 5001 :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
SELECT ?p ?o
WHERE {
?pheno a nav:PhenomeneMeteorologiqueOuOceanographique.
?pheno nav:estLocaliseA ent:5001.
?pheno ?p ?o.
}
```

Quels sont les horaires des renverses au mouillage extérieur de Roscoff ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
SELECT DISTINCT ?temporalité ?temps ?portRattachement
WHERE {
?s a nav:Renverse.
?s nav:estLocaliseA ?lieu.
    ?lieu rdfs:label ?nomLieu.
    FILTER regex(str(?nomLieu), "mouillage extérieur de Roscoff")
?s nav:aPourTemporaliteQuantitative ?temps.
        ?s ?temporalité ?temps.
?s nav:aPourPortDeRattachement ?port.
?port rdfs:label ?portRattachement.
}
```

Quels sont les courants ou vagues dont il faut tenir compte dans le site 5008 ?
Pour avoir les informations de tous les phénomènes océanographiques dans le site 5008 :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
SELECT distinct ?s ?p ?o ?p2 ?o2 ?p3 ?o3
WHERE {
?s a nav:PhenomeneOceanographique.
?s nav:estLocaliseA ent:5008.
?s ?p ?o.
    OPTIONAL {<<?s ?p2 ?o2>> ?p3 ?o3}
}
```

Est-ce que les conditions météo affectent la marée à Dunkerque ?
Pour avoir toutes les conditions météorologiques à Dunkerque qui ont comme conséquence quelque chose qui est lié à la marée :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
SELECT distinct ?s ?p ?o ?c
WHERE {
?s a nav:PhenomeneMeteorologique.
?s ?p ?o.
?s nav:aPourConsequence ?c.
Filter regex(?c, "marée")
}
```

Quelles sont les vitesses des courants au large du Cap Blanc-Nez ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
SELECT DISTINCT ?s ?vitesse ?typeDeVitesse ?p1 ?v1 ?lieu2
WHERE {
?s a nav:Courant.
?s nav:estAuLargeDe ?lieu.
?lieu a nav:EntiteGeographique.
?lieu rdfs:label "Cap Blanc-Nez"@fr.
    OPTIONAL {?s nav:aPourVitesse ?vitesse.
    <<?s ?typeDeVitesse ?vitesse>> ?p1 ?v1}
?s nav:estLocaliseA ?lieu2
}
```

Y-a-t-il des courants giratoires autour de Douarnenez ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX qudt: <http://qudt.org/schema/qudt/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX tcr: <http://data.shom.fr/id/codes/nav/typedecourant/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
SELECT DISTINCT ?courantGiratoire ?propriété ?nomLieu
WHERE {
?courantGiratoire a nav:Courant.
?courantGiratoire nav:aPourTypeDeCourant tcr:CourantGiratoire.
?courantGiratoire nav:estLocaliseA ?ent.
?ent nav:aUneRelationSpatialeAvec ?lieu.
?ent ?propriété ?lieu.
    ?lieu rdfs:label ?nomLieu
	FILTER (regex(str(?nomLieu), "Douarnenez" ))
}
```

Quels sont les consignes pour les petits navires pour entrer dans le Canal de l'Île de Batz ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
SELECT DISTINCT ?ent ?type ?p ?o
WHERE {
?ent a nav:ConsigneDeNavigation.
?ent nav:aPourPointDeDestination ?nb1.
?nb1 rdf:member ?lieu.
?lieu rdfs:label "Canal de l'Île de Batz"@fr.
?ent nav:impliqueDeSuivre ?nb2.
?nb2 rdf:member ?suivre.
?suivre ?p ?o.
?ent nav:aPourCible ?navire.
?navire a nav:Navire.
?navire nav:aPourTaille tta:Petit
}
```

Quels navires peuvent mouiller dans le port de Camaret-sur-Mer ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
SELECT ?nombreDePlaces ?proprieteNavire ?objetNavire ?proprieteNavire2 ?objetNavire2
WHERE {
?ent nav:aPourNature teg:Port.
?ent rdfs:label ?nom.
    FILTER (regex(str(?nom), "Camaret-sur-Mer"))
    OPTIONAL {?ent nav:aPourNombreDePlaces ?nombreDePlaces.}
    OPTIONAL {<<?ent nav:aPourNombreDePlaces ?nombreDePlaces>> nav:aPourCible ?cible.
				?cible ?proprieteNavire ?objetNavire.}
    OPTIONAL {<<?cible ?proprieteNavire ?objetNavire>> ?proprieteNavire2 ?objetNavire2}
}
```

Pour quels navires est le pilotage obligatoire dans le zone de pilotage de Brest ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
SELECT DISTINCT ?proprieteCible ?objetCible ?proprieteConsigne ?objetConsigne
WHERE {
?ent nav:aPourNature teg:ZoneDePilotage.
    ?ent nav:estSitueDans ?endroit.
    ?endroit rdfs:label ?nom
    FILTER (regex(str(?nom), "Brest" ))
?consigne nav:aPourLieuDEffet ?ent.
    ?consigne a nav:ConsigneDeNavigation.
    ?consigne nav:aPourCible ?cible.
	?cible ?proprieteCible ?objetCible.
    ?consigne ?proprieteConsigne ?objetConsigne.
}
```

Est-ce que les navires étrangers à l’Union européenne sont admis à relâcher aux Îles Chausey ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
PREFIX tet: <http://data.shom.fr/id/codes/nav/typedetat/>
SELECT DISTINCT ?p ?o
WHERE {
?ent a nav:EntiteGeographique.
     ?ent rdfs:label "Îles Chausey"@fr.
?consigne nav:aPourLieuDEffet ?ent.
    ?consigne a nav:ConsigneDeNavigation.
    ?consigne nav:aPourCible ?cible.
?consigne ?p ?o.
?cible a nav:Navire.
    ?cible nav:aPourEtat tet:EtrangerALUE
}
```

Est-ce que les navires de plaisance peuvent emprunter le Passage du Fromveur ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
PREFIX tet: <http://data.shom.fr/id/codes/nav/typedetat/>
SELECT DISTINCT ?p ?o
WHERE {
?ent a nav:EntiteGeographique.
     ?ent rdfs:label "Passage du Fromveur"@fr.
?consigne nav:aPourLieuDEffet ?ent.
    ?consigne a nav:ConsigneDeNavigation.
    ?consigne nav:aPourCible ?cible.
?consigne ?p ?o.
?cible nav:estDeType tna:NavireDePlaisance.
}
```

Comment peut un navire qui n'est pas équipé de VHF obtenir un poste portatif dans la Seine maritime ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
PREFIX tet: <http://data.shom.fr/id/codes/nav/typedetat/>
PREFIX teq: <http://data.shom.fr/id/codes/nav/typedequipement/>
SELECT DISTINCT ?p ?o
WHERE {
?ent a nav:EntiteGeographique.
     ?ent rdfs:label "Seine maritime"@fr.
?consigne nav:aPourLieuDEffet ?ent.
    ?consigne a nav:ConsigneDeNavigation.
    ?consigne nav:aPourCible ?cible.
	?consigne ?p ?o.
?cible a nav:Navire.
    ?cible nav:nEstPasEquipeDe teq:VHF.
}
```