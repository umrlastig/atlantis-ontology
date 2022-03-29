# Argumentaire du modelet Entités

## Nom
Entités pérennes de l'environnement maritime côtier et relations spatiales

## Description
Les _Instructions nautiques_ contiennent des références à des entités pérennes de l'environnement maritime côtier et à des relations spatiales. Une entité pérenne de l'environnement maritime côtier peut être une entité géographique ou une aide virtuelle à la navigation. Les entités pérennes de l'environnement maritme côtier sont cités dans les _Instructions nautiques_ dans les descriptions de paysages, dans les consignes de navigation, dans les règlements et dans les descriptions de phénomènes météorologiques et océanographiques. Les relations spatiales sont cités dans les _Instructions nautiques_ dans les descriptions des positions d'entités pérennes de l'environnement maritime côtier ou de phénomènes météorologiques et océanographiques, ou bien dans les consignes de navigation.

Une entité géographique est une entité physique, visible à l’œil. Une entité géographique peut être soit naturelle (p. ex. basse, passe, rive, fleuve, île), soit artificielle (p. ex. brise-lames, chapelle, clocher, pyramide, sas) ou encore administrative (p. ex. département, parc régional, ville) [https://toponymie.gouv.qc.ca/ct/normes-procedures/terminologie-geographique/entite.aspx]. Une entité géographique peut être soit dans le domaine terrestre (p. ex. maison, pointe, zone industriel), soit dans le domaine maritime (p. ex. anse, balise, haut fond), soit les deux (soit invariable selon son emplacement, p. ex. roche, Zone prioritaire pour la biodiversité ; soit variable selon la marée, p. ex. estran). La taille et la position d'une entité géographique peut être concrète (p. ex. pyramide, département, phare) ou floue (p. ex. couloir, passe d'entrée, zone d'attente). Les entités géographiques peuvent être utilisées pendant une navigation pour se situer localement.

Une aide virtuelle à la navigation n'est pas une entité physique et n'est pas visible à l’œil. Une aide virtuelle à la navigation peut être un alignement, un dispositif de séparation du trafic (DST), un relèvement, un repérage, une route ou un secteur. Les aides virtuelles à la navigation peuvent être utilisées pour aider à décrire un itinéraire de navigation.

Une relation spatiale implique au moins deux entités pérennes de l'environnement maritime côtier ou phénomènes météorologiques ou océanographiques, dont au moins une doit être une entité pérenne de l'environnement maritime côtier. Les relations spatiales aident à situer les entités pérennes de l'environnement maritime côtier et les phénomènes météorologiques ou océanographiques en mer ou sur une carte marine. Une relation spatiale peut être concrète (la zone de mouillage est à l'Est de la jetée) ou floue (l'île est entourée de dangers). Une relation spatiale peut avoir une orientation cardinale et/ou une orientation angulaire. Une relation spatiale peut impliquer une distance. Toutes relations spatiales sont transitives (p. ex., si la bouée A est à l'Ouest de la bouée B et la bouée B est à l'Ouest de la bouée C, on peut dire que la bouée A est à l'Ouest de la bouée C) et certaines sont également inversables (p. ex., si la balise A est au Sud de la balise B, on peut dire que la balise A est au Nord de la balise B ; cependant si la tourelle C est dans l'Est de la zone D, on ne peut pas dire que la zone D est dans l'Ouest de la tourelle C).

Chaque entité pérenne de l'environnement maritime côtier est caractérisé par :
* {obligatoire} sa nature
    * {optionnel} si elle est un type de danger
    * {optionnel} si elle est un type de lieu de stationnement
* {optionnel} son nom
* {optionnel} ses coordonnées géographiques
* {optionnel} les relations spatiales entre elle et d'autres entités ou phénomènes
    * {optionnel} les entités qui la marquent
    * {optionnel} les entités qu'elle marque
* {optionnel} les entités dont elle est un élément
* {optionnel} les entités dont elle est composée
* {optionnel} son hauteur, avec unités
* {optionnel} sa largeur, avec unités
* {optionnel} sa couleur ou ses couleurs
    * {optionnel} le motif des couleurs
* {optionnel} sa forme
* {optionnel} le type de marque
    * {optionnel} son type cardinal
    * {optionnel} son type latéral
* {optionnel} la profondeur de l'eau, avec unités
    * {optionnel} la profondeur minimun de l'eau, avec unités
    * {optionnel} la profondeur maximum de l'eau, avec unités
* {optionnel} la hauteur verticale découverte de l'eau, avec unités
* {optionnel} la nature du fond
* {optionnel} l'entité géographique ou l'organisation qui la gère
* {optionnel} des informations complémentaires
* {optionnel} ses angles de début et de fin, avec unités
* {optionnel} son cap, avec unités
* {optionnel} le nombre de places de stationnement disponibles
* {optionnel} si elle est equipée d'une balise AIS
* {optionnel} si elle est un repère lumineux

Chaque relation spatiale est caractérisée par :
* {obligatoire} les entités ou phénomènes impliquées

## Exemples
### Exemple 1
"Vue du Nord, l’Île de Batz montre la tour du sémaphore et surtout le phare, tour grise haute de 43 m, entourée de maisons. Ce phare est équipé d’une balise d’émission AIS. L’île est débordée de tous côtés par des dangers. Les plus au large sont : à l’Est, la Basse Astan, couverte de 0,8 m d’eau, marquée par la bouée « Astan », cardinale Est lumineuse ; au Nord, la Grande Basse, couverte de 0,5 m d’eau ; à l’Ouest, Men Aodi, roche non balisée découvrant de 0,1 m." [C2A, p. 528]

### Exemple 2
"Le Canal de l’Île de Batz est un chenal profond de 0,1 à 10 m qui sépare l’Île de Batz de la côte et donne accès aux ports d’échouage de Porz Kernok (Île de Batz) et de Roscoff (§ 9.4.3.6.). On ne doit s’y engager qu’avec une bonne connaissance des lieux et le concours d’un pratique local." [C2A, p. 528]

### Exemple 3
"MOUILLAGES D’ATTENTE. — Ces mouillages, utilisés notamment par les navires se rendant à Roscoff, se trouvent dans l’Est et dans l’Ouest du chenal. Un des meilleurs se trouve au NE de la tourelle « Men Guen Bras », par profondeur de 14 m, fond de sable et coquille de bonne tenue. Prendre garde à la roche couverte de 2,8 m située à 0,3 M à l’ENE de la tourelle.
Par vents d’Est, on peut mouiller partout dans la partie Ouest du chenal jusqu’au Sud de la tourelle « Malvoch », implantée près de l’extrémité de la jetée de Porz Kernok." [C22, p. 400]

### Exemple 4
"PORT DE L’ÎLE DE BATZ (Porz Kernok) [48° 44,6' N — 4° 00,8' W]. — Ce port d’échouage est géré par le département du Finistère. Situé sur la côte Sud de l’Île de Batz et bien protégé de tous les vents, il sert d’abri aux pêcheurs de l’île." [C2A, p. 529]

### Exemple 5
"La Pointe de Bloscon porte la chapelle de Sainte-Barbe (48° 43,6' N — 3° 58,2' W), de couleur blanche ; plus au SW on voit le clocher de Roscoff et, juste au Sud, les installations portuaires de Roscoff-Bloscon. À 3 M au SW du phare de Batz, l’Île de Siec comporte, près de son extrémité Ouest, une petite anse ouverte au Sud, protégée à l’Ouest par un môle." [C2A, p. 530]

### Exemple 6
"Moguériec (48° 41,3' N — 4° 04,3' W) est abrité au Nord par une jetée. Ce port offre un abri précaire aux pêcheurs et aux plaisanciers locaux. [...]
À l’abri de la jetée débouche un ruisseau bordé d’un quai de chaque côté. Sur la rive Nord se trouve un terre-plein et deux escaliers. Les posées, sur sable plat, sont franches partout sauf en bordure de la jetée ; les fonds découvrent de 4 à 5 m, voire de plus de 7 m à l’embouchure du ruisseau. La plupart des places à quai sont occupées par des bateaux de pêche qui y béquillent ; les bateaux de plaisance échouent entre le terre-plein et le milieu de la jetée." [C2A, p. 531]

### Exemple 7
"L’échouage de Porz Guen (48° 39,89' N — 4° 13,07' W) est protégé à l’Ouest par une digue et au Sud par un brise-lames submersible en enrochements. Il sert d’abri aux bateaux de pêche, par des fonds découvrant de 2 à 5,5 m.
Le port dispose d’une cale enracinée à un terre-plein et offre une vingtaine de places sur bouées. La passe d’entrée est marquée par deux balises latérales." [C22, p. 404-405]

### Exemple 8
"CHENAL DE LA MALOUINE. INSTRUCTIONS. — Ce chenal, profond de 3 m, n’a que 100 m de largeur entre le plateau de La Malouine et celui de La Pendante." [C22, p. 411]

### Exemple 9
"9.4.5.5. Port de l’Aber-Wrac’h
L’Aber-Wrac’h (48° 35,9' N — 4° 33,7' W), établi sur la rive gauche de l’aber, entre l’Anse des Anges et l’Anse Saint-Antoine, est un port de plaisance et de pêche géré par la chambre de commerce et d’industrie de Brest.
[...]
Le mouillage de Karreg Du se trouve entre les tourelles de la Roche aux Moines et le port." [C2A, p. 537]

### Exemple 10
"Deux tourelles portant chacune un feu marquent, entre la chaussée et Guernsey, les rochers Roustel et Platte ; la première (49° 29,23' N — 2° 28,79' W) est tronconique à damier noir et blanc avec lanterne verte, la seconde (49° 29,09' N — 2° 29,57' W) est conique verte." [C22, p. 180]