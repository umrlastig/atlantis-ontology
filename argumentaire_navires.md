# Modelet : Navires

## Scénario de motivation

**Nom :** Navires

**Dernière mise à jour :** 21 juillet 2021

**ID entités géographiques :** ent:3000

**Description :** Les consignes de navigation fournies dans les Instructions Nautiques indiquent parfois pour quels types de navires elles sont valides. Selon le type de navire, les consignes seront donc différentes. Ces informations ne figurent pas sur les cartes marines et sont recherchées par les navigateurs dans les IN lorsqu'ils préparent leur mission.

La description de chaque navire est caractérisé par :

* {optionnel} type de navire
* {optionnel} ce dont il est/il n'est pas équipé
* {optionnel} cargaison
* {optionnel} taille qualitative
* {optionnel} état
* {optionnel} port en lourd
* {optionnel} capacité
    * {optionnel} jauge brute
    * {optionnel} tonnage
* {optionnel} dimension quantitative
    * {optionnel} calaison
    * {optionnel} tirant d'air
    * {optionnel} tirant d'eau
    * {optionnel} largeur
    * {optionnel} longueur
    * {optionnel} longueur hors-tout
* {optionnel} déplacement
* {optionnel} rayon de giration
* {optionnel} vitesse

**Exemple 1 :** "En venant de l’Est, on prend le chenal en suivant l’alignement à 293,3° du clocher de l’Île de Batz (chapelle Notre-Dame de Bon Secours), sur la côte Sud de l’île, par la pyramide blanche de l’Île Pigued (48° 44,0' N — 3° 58,2' W). Cet alignement n’est visible par les petits navires que jusqu’à environ 0,6 M à l’Est de la tourelle « Le Menk » (à mi-marée) et, par les navires à passerelle plus haute, jusqu’au Nord de la tourelle ; il se situe dans le secteur blanc (289,5° – 293°) du feu de la tourelle « Ar Chaden » (§ 9.3.3.1.). La route à 293,3° laisse au Nord le Plateau des Duons et au Sud Bazenn ar Menk (tourelle « Le Menk », cardinale Ouest lumineuse), et la Basse de Bloscon (bouée cardinale Nord lumineuse).
Les petits navires d’où il n’est pas possible de voir le clocher de l’Île de Batz, masqué par la végétation, peuvent se présenter légèrement à gauche de l’alignement de garde à 290° du phare de l’Île de Batz par la tourelle « Ar Chaden »."

**Exemple 2 :** "Les principaux équipements et services offerts sont les suivants : 550 places pour navires de plaisance, dont 150 pour les bateaux de passage, longueur maximum 15 m, tirant d’eau 5 m ; 60 places sur corps-morts ; [...]"

**Exemple 3 :** "Le pilotage est également obligatoire pour tous les navires transportant des hydrocarbures ou des substances dangereuses, quelles que soient leurs dimensions."

**Exemple 4 :** "AVERTISSEMENT. — Les navires étrangers à l’Union européenne ne sont pas admis, sauf cas de force majeure dûment constaté, à relâcher aux Îles Chausey où n’existe pas de service de douane permanent."

**Exemple 5 :** "Le passage est rectiligne, facile à suivre et avantageux par beau temps, lorsque l’on a le courant pour soi. Mais les petits bâtiments (navires de pêche et de plaisance, et les navires de faible puissance) doivent prendre de très grandes précautions pour franchir ce passage, même par de bonnes conditions de temps et de courant."

**Exemple 6 :** "Pour obtenir un poste portatif, les navires qui ne sont pas équipés de VHF doivent le signaler dans le message d’arrivée pour les navires entrants ou lors des demandes de départ pour les navires sortants."

## Informal competency questions

**Identifiant : 1**

Question : Quels sont les consignes pour les petits navires dans le Canal de l'Île de Batz ?

Résultat attendu : Les consignes de navigation qui sont spécifiques pour les petits navires dans le Canal de l'Île de Batz.

Exemple : En venant de l’Est, on prend le chenal en se présentant légèrement à gauche de l’alignement de garde à 290° du phare de l’Île de Batz par la tourelle « Ar Chaden ».

Dépend de : /

**Identifiant : 2**

Question : Quels navires peuvent mouiller dans le port de Camaret-sur-Mer ?

Résultat attendu : La liste des types de navires qui peuvent mouiller dans le port de Camaret-sur-Mer ainsi que leurs caractéristiques.

Exemple : Navires de plaisance et bateaux de passage, longueur maximum 15 m, tirant d’eau 5 m.

Dépend de : /

**Identifiant : 3**

Question : Pour quels navires est le pilotage obligatoire dans le zone de pilotage de Brest ?

Résultat attendu : La liste des types de navires pour lesquels le pilotage est obligatoire.

Exemple : Tous les navires transportant des hydrocarbures ou des substances dangereuses

Dépend de : /

**Identifiant : 4**

Question : Est-ce que les navires étrangers à l’Union européenne sont admis à relâcher aux Îles Chausey ?

Résultat attendu : La liste des conditions sous lesquelles les navires étrangers à l’Union européenne sont admis à relâcher aux Îles Chausey.

Exemple : Les navires étrangers à l’Union européenne ne sont pas admis, sauf cas de force majeure dûment constaté, à relâcher aux Îles Chausey où n’existe pas de service de douane permanent.

Dépend de : /

**Identifiant : 5**

Question : Est-ce que les navires de plaisance peuvent emprunter le Passage du Fromveur ?

Résultat attendu : La liste des consignes pour la navigation des navires de plaisance dans le passage.

Exemple : Les navires de plaisance doivent prendre de très grandes précautions pour franchir ce passage, même par de bonnes conditions de temps et de courant.

Dépend de : /

**Identifiant : 6**

Question : Comment peut un navire qui n'est pas équipé de VHF obtenir un poste portatif dans la Seine maritime ?

Résultat attendu : La liste des consignes pour un navire sans VHF d'obtenir un poste portatif.

Exemple : Pour obtenir un poste portatif, les navires qui ne sont pas équipés de VHF doivent le signaler dans le message d’arrivée pour les navires entrants ou lors des demandes de départ pour les navires sortants.

Dépend de : /

## Glossaire des termes

**Terme :** Navire

**Définition :** Un navire est toute type d'embarcation ou engin flottant sur l'eau, y compris les barques, les bateaux, les bâtiments, les paquebots, les pétroliers et les vaisseaux. Un navire peut être militaire, commercial, public ou privé. Un navire peut être équipé de divers équipements et un navire de commerce peut transporter diverses cargaisons. À tout moment, un navire peut être dans un état donné, par exemple être à faible puissance, être étranger (par rapport au pays dans lequel il se trouve), être en réparation ou être mouillé.

**Terme :** Équipement

**Définition :** Un navire peut être équipé de divers équipements. Un équipement est un élément d'un navire qui ne fait pas partie de son cargaison, par exemple un radar, une installation VHF ou un propulseur d'étrave.

**Terme :** Cargaison

**Définition :** Un navire de commerce peut transporter diverses cargaisons. La cargaison d'un navire de commerce est l'ensemble des marchandises chargées à bord.

**Terme :** État

**Définition :** À tout moment, un navire peut être dans un état donné, par exemple être à faible puissance, être étranger (par rapport au pays dans lequel il se trouve), être en réparation ou être mouillé.

**Terme :** Port en lourd

**Définition :** Le port en lourd d'un navire est la différence exprimée en tonnes métriques (1000 kg) ou en "long tons" (1016 kg) entre le déplacement du navire lège et son déplacement à pleine charge. (Source : http://www.umnp.org/index.php?option=com_glossary&func=view&Itemid=75&catid=13&term=PORT+EN+LOURD+(Deadweight))

**Terme :** Déplacement

**Définition :** La déplacement d'un navire est le poids d'eau déplacé par le navire en tonnes métriques (1000 kg) ou en long tons (1016 kg). On distingue le déplacement lège qui est le poids du navire non chargé, le déplacement en charge qui est le poids du navire chargé au maximum. La différence entre les deux est le port en lourd total. (Source : http://www.umnp.org/index.php?option=com_glossary&func=view&Itemid=75&catid=13&term=DEPLACEMENT+%28Displacement%29+)

**Terme :** Capacité

**Définition :** La capacité d'un navire peut être mesurée par sa jauge brute ou par son tonnage.

**Terme :** Jauge brute

**Définition :** La jauge brute d'un navire est sa capacité au-dessous du pont. La jauge brute est un mesure officielle des capacités intérieures des navires. L'unité de la jauge brute est le tonneau de jauge (gross ton, register ton) (2,83 m^3 ou 100 cft). (Source : http://www.umnp.org/index.php?option=com_glossary&func=view&Itemid=75&catid=13&term=JAUGE+%28Tonnage%29+)

**Terme :** Tonnage

**Définition :** Le tonnage représente la capacité de transport d'un navire de commerce, évaluée par son volume intérieur exprimé en tonneaux de jauge (2,83 m^3 ou 100 cft). Tonnage est un synonyme de jauge. Le tonnage brut représente la capacité intérieure totale d'un navire. Le tonnage net représente la capacité intérieure d'un navire utilisable commercialement. (Source : https://www.cnrtl.fr/lexicographie/tonnage)

**Terme :** Calaison

**Définition :** La calaison est l'enfoncement d'un navire en raison de son chargement. Calaison est un synonyme de tirant d'eau. (Source : https://www.cnrtl.fr/definition/calaison)

**Terme :** Tirant d'air

**Définition :** Le tirant d'air d'un navire est la hauteur maximale des superstructures ou des mâts d'un bateau, au-dessus de la ligne de flottaison. (Source : https://fr.wikipedia.org/wiki/Tirant_d%27air)

**Terme :** Tirant d'eau

**Définition :** Le tirant d'eau d'un navire est la distance verticale entre la surface et le point le plus bas d'un navire (quille ou appendice de coque). C'est le tirant d'eau qui conditionne la sécurité de la navigation. (Source : http://iho-ohi.net/S32/engFreView.php)

**Terme :** Largeur

**Définition :** La largeur d'un navire correspond à la distance entre les points extrêmes bâbord et tribord de la structure permanente du bateau.

**Terme :** Longueur

**Définition :** La longueur d'un navire se mesure à partir du devant de la proue jusqu'à l'arrière de la poupe. Elle correspond à la distance entre les points extrêmes avant et arrière de la structure permanente du bateau. Cette mesure n'inclut pas les éléments attachés à l'embarcation comme les échelles de bains et les moteurs hors-bord. (Source : https://cartebateau.com/fr/longueur-d-un-bateau-hors-tout)

**Terme :** Longueur hors-tout

**Définition :** La longueur hors-tout d'un navire correspond à la distance entre les points extrêmes avant et arrière de la structure permanente du bateau. Ceci inclut les éventuels espars tels que le beaupré ou une queue de malet ainsi que les balcons. Cette mesure inclut les éléments attachés à l'embarcation comme les échelles de bains et les moteurs hors-bord. (Sources : https://cartebateau.com/fr/longueur-d-un-bateau-hors-tout, https://fr.wikipedia.org/wiki/Longueur_hors-tout)

**Terme :** Rayon de giration

**Définition :** Le rayon de giration d'un navire correspond au rayon maximal du cercle sur la surface de l'eau dans lequel le navire est mobile lorsqu'il est mouillé à l'ancre, où le centre du cercle est directement au dessus de la position de l'ancre sur le fond marin. Le rayon de giration d'un navire mouillé peut être calculé à partir de mesures de la profondeur de l'eau et de la longueur de la chaîne d'ancre.

**Terme :** Vitesse

**Définition :** La vitesse d'un navire est mesuré en nœuds. Un nœud correspond à 1 mille par heure (1,852 km/h).


## **Requêtes SPARQL**

**Q1 :** Quels sont les consignes pour les petits navires dans le Canal de l'Île de Batz ?
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
SELECT DISTINCT ?ent ?s ?nom ?p ?o ?ou ?lieu ?navire
WHERE {
?ent a nav:ConsigneDeNavigation.
    OPTIONAL { ?ent nav:impliqueDeSuivre ?nb.
    ?nb rdf:member ?s.
?s a ?nom}
?ent ?p ?o.
?ent ?ou ?lieu.
?lieu rdfs:label "Canal de l'Île de Batz"@fr.
?ent nav:aPourCible ?navire.
?navire a nav:Navire.
?navire nav:aPourTaille tta:Petit.
}
```

**Q2 :** Quels navires peuvent mouiller dans le port de Camaret-sur-Mer ?
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

**Q3 :** Pour quels navires est le pilotage obligatoire dans le zone de pilotage de Brest ?
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

**Q4 :** Est-ce que les navires étrangers à l’Union européenne sont admis à relâcher aux Îles Chausey ?
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

**Q5 :** Est-ce que les navires de plaisance peuvent emprunter le Passage du Fromveur ?
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

**Q6 :** Comment peut un navire qui n'est pas équipé de VHF obtenir un poste portatif dans la Seine maritime ?
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