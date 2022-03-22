# Modelet : Temporalité et phénomènes météorologiques et océanographiques

## Scénario de motivation

**Nom**: Temporalité et phénomènes météorologiques et océanographiques

**Dernière mise à jour :** 21 juillet 2021

**ID entités géographiques :** (ent:5000)

**Description :** Les _Instructions Nautiques_  contiennent des références à la temporalité ainsi qu'à des phénomènes météorologiques et océanographiques. Les IN peuvent décrire l'existence de phénomènes météorologiques ou océanographiques en fonction de leur position et/ou leur temporalité. Les consignes de navigation fournies dans les IN peuvent dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, ce qui veut dire que les consignes peuvent varier en conséquence de ces conditions locales. Toutes ces informations ne figurent pas sur les cartes marines et sont recherchées par les navigateurs dans les IN lorsqu'ils préparent leur mission.

La description de chaque phénomène météorologique ou océanographique, est caractérisée par :

* {obligatoire} lieu d'effet
* {optionnel} conséquence : sur l'environnement / sur les consignes de navigation
* {optionnel} temporalité

Les phénomènes météorologiques affectent généralement l'état de la mer.

**Exemple 1 :** "Dans le milieu du chenal, les renverses ont lieu vers – 0525 et + 0020 PM Roscoff. Le flot porte à l’Est et le jusant à l’Ouest ; les vitesses varient selon les endroits, mais sont de 2,5 à 3,5 nœuds en général. Le courant est traversier à l’entrée Est du chenal, à l’Est de la ligne joignant l’Île Pigued à la tourelle « Men Guen Bras ».

Aux abords de Roscoff, le jusant porte à l’Ouest et le flot à l’Est. Il y a étale du courant vers – 0050 PM Roscoff. Au mouillage extérieur de Roscoff, entre la tourelle « Le Menk » et la côte, les renverses ont lieu à – 0050 et à + 0550 PM Roscoff. Le flot porte à 185°, le jusant à 351° ; les vitesses sont de 1,1 nœud."

**Exemple 2 :** "Le site est exposé au ressac par mauvais temps de Nord à NE."

**Exemple 3 :** "Par vents de NE, on constate souvent une réduction des hauteurs de marée pouvant dépasser 0,3 m. Les vents des autres secteurs font apparaître, au contraire, une surélévation de 0,5 m ou plus."

**Exemple 4 :** "Au large et à l’Est du méridien du Cap Blanc-Nez, le courant porte au large à la fin du flot et à terre à la fin du jusant. Au large, les vitesses maximales en VE moyenne atteignent 1,7 nœud sur les bancs ou à proximité et 2,9 nœuds dans les passes et entre les bancs. Le flot portant au NE est plus fort mais dure moins longtemps que le jusant qui porte au SW."

## Informal competency questions

**Identifiant: 1**

Question: Quels sont les phénomènes météorologiques ou océanographiques qui affectent la navigation dans la zone X?

Résultat attendu: La liste des phénomènes météorologiques ou océanographiques qui affectent la navigation dans la zone X

Exemple: Dans le milieu du chenal: les renverses, le flot, le jusant. A l'entrée Est du chenal: le courant traversier. Sur le site X, le mauvais temps. Sur la zone Y, les vents de NE.

Dépend de: /

**Identifiant : 1.2**

Question: Quels sont les horaires des renverses au mouillage extérieur de Roscoff ?

Résultat attendu: Les horaires des renverses au mouillage extérieur de Roscoff ainsi que le port d'attachement.

Exemple: – 0050 et à + 0550 PM Roscoff

**Identifiant: 2**

Question: Quels sont les courants dont il faut tenir compte dans la zone X?

Résultat attendu: La liste des courants dont il faut tenir compte et leurs caractéristiques (direction et vitesse par exemple)

Exemple: le flot, direction Est, vitesse entre 2.5 et 3.5 noeuds et le jusant, direction Ouest, vitesse entre 2.5 et 3.5 noeuds.

Dépend de: 1

**Identifiant: 3**

Question: Est-ce que les conditions météo affectent la marée dans la zone X?

Résultat attendu: La liste des phénomènes météo qui peuvent affecter la marée dans la zone X et leurs conséquences.

Exemple: Vents de NE --> réduit les hauteurs de marées de min 0.3 m et Autres vents --> augmente les hauteurs de marées de min 0.5 m.

Dépend de: 1

**Identifiant : 4**

Question : Quelles sont les vitesses des courants au large du Cap Blanc-Nez ?

Résultat attendu : La liste des vitesses des courants au large du Cap Blanc-Nez.

Exemple : Au large du Cap Blanc-Nez, les vitesses maximales en VE moyenne atteignent 1,7 nœud sur les bancs ou à proximité et 2,9 nœuds dans les passes et entre les bancs.

**Identifiant : 5**

Question : Y-a-t-il des courants giratoires autour de Douarnenez ?

Résultat attendu : La liste des courants giratoires autour de Douarnenez et les informations associées.

Exemple : À mesure que l’on se rapproche de la terre, le courant giratoire diminue mais reste encore sensible à l’Ouest du Goulet de Brest et de la Baie de Douarnenez.


## Glossaire des termes

**Terme:** Courant

**Définition:** Le mouvement permanent ou périodique des eaux, généralement dans le sens horizontal, dû à diverses causes telles que des différences de température, le vent ou les marées.

**Terme:** Courant de marée

**Définition:** Le mouvement permanent ou périodique des eaux, généralement dans le sens horizontal, dû aux marées.

**Terme:** Courant dû au vent

**Définition:** Le mouvement permanent ou périodique des eaux, généralement dans le sens horizontal, dû au vent.

**Terme:** Flot

**Définition:** Le courant de flot est le courant créé par la marée montante. Le flot ne coïncide pas exactement avec la marée montante.

**Terme:** Jusant

**Définition:** Le courant de jusant est le courant créé par la marée descendante. Le le jusant ne coïncide pas exactement avec la marée descendante.

**Terme:** Renverse

**Définition:** Entre le flot et le jusant, le courant devient nul durant une période variable selon le lieu : c'est l'étale ou renverse.

**Terme:** Indication Météorologique Qualitative

**Définition:** Précision informelle de l'état général de la météo, exprimée en langage nat : "par mauvais temps" "par temps de brume"

**Terme:** Vent

**Définition:** Phénomène caractérisé par un déplacement d'air plus ou moins important, de direction variable, dans les couches élevées de l'atmosphère comme à la surface du globe.

**Terme:** direction

**Définition:** Ligne qu'une personne se propose de suivre ou suivant laquelle un corps mobile ou un objet qui se déplace, se dirige ou est dirigé.

**Terme:** vitesse

**Définition:** Espace parcouru en fonction du temps mis à le parcourir.

**Terme:** force

**Définition:** la force du vent selon l'échelle Beaufort. L'échelle Beaufort est une échelle de mesure empirique, comportant 13 degrés (de 0 à 12), de la vitesse moyenne du vent sur une durée de dix minutes utilisée dans les milieux maritimes.

**Terme:** localisé à

**Définition:** Lieu où se situe un phénomène météorologique ou océanographique désigné par référence à une entité géographique, désignée par son nom ou son type, une carte ou bien par référence à des coordonnées.

**Terme:** a pour conséquence

**Définition:** conséquence de la survenue d'un phénomène météorologique ou océanographique sur l'état de l'environnement hydrographique ou sur les consignes de navigation, telle que mentionnée dans le texte des IN. **Attention!** Dans le cas des conséquences sur les consignes de navigation, penser à vérifier à terme si ce n'est pas équivalent à la partie *Requirement* des règles (*Rules*) définies dans l'ontologie présentée là: Hagaseth, M., Lohrmann, P., Ruiz, A., Oikonomou, F., Roythorne, D. and Rayot, S., 2016. An ontology for digital maritime regulations. *Journal of Maritime Research*, *13*(2). Idem pour a pour temporalité \~ *Context* ?

**Terme:** a pour temporalité

**Définition:** le caractère temporel du phénomène météorologique ou océanographique, désigné par l'heure ou bien les horaires de pleine mer d'un port de référence ou encore une indication temporelle qualitative (ex: "à mi-marée").

## **Requêtes SPARQL**

**Q1 :** Quels sont les phénomènes météorologiques ou océanographiques qui affectent la navigation dans le milieu du chenal 5001 ?
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
NB: A terme, quand on introduira GeoSPARQL, remplacer ici EntiteGeographique par SpatialObject pour permettre de requêter à la fois sur des lieux nommés et sur des polygones ou des BBOX.

**Q1.2 :** Quels sont les horaires des renverses au mouillage extérieur de Roscoff ?
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
Fonctionne uniquement avec inference.

**Q2 :** Quels sont les courants ou vagues dont il faut tenir compte dans le site 5008 ?
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
Fonctionne uniquement avec inference.

**Q3 :** Est-ce que les conditions météo affectent la marée à Dunkerque ?
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
Fonctionne uniquement avec inference.

**Q4 :** Quelles sont les vitesses des courants au large du Cap Blanc-Nez ?
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

**Q5 :** Y-a-t-il des courants giratoires autour de Douarnenez ?
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
Pourquoi rdf:type un node blanc ?
Fonctionne uniquement avec inference.