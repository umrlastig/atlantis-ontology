# Modelet : Entités pérennes du paysage maritime côtier et relations spatiales

## Scénario de motivation

**Nom :** Entités pérennes du paysage hydrographique côtier et relations spatiales

**Dernière mise à jour :** 21 juillet 2021

**ID entités géographiques :** (ent:4000)

**Description :** Les _Instructions nautiques_  contiennent des références à des entités pérennes du paysage hydrographique côtier et à des relations spatiales entre eux. Une entité pérenne du paysage hydrographique côtier peut être une entité géographique ou un groupe d'entités géographiques. Les entités pérennes du paysage hydrographique côtier sont cités dans les IN dans les descriptions de paysages, dans les consignes de navigation, dans les règlements et dans les descriptions de phénomènes météorologiques et océanographiques. Les entités pérennes du paysage hydrographique côtier sont utilisées pendant une navigation pour se situer localement.

Une entité géographique peut être soit naturelle (basse, fleuve, passe, raz, rive, roche, île), soit artificielle (brise-lames, cale, chapelle, clocher, digue, débarcadère, escalier, estacade, jetée, pyramide, quai, sas, sémaphore, terre-plein, tour) ou encore administrative (département, parc régional, ville) (source : https://toponymie.gouv.qc.ca/ct/normes-procedures/terminologie-geographique/entite.aspx). Une entité géographique peut être soit dans le domaine terrestre (maison, pointe, zone industriel), soit dans le domaine maritime (anse, balise, haut fond), soit les deux (invariable selon son emplacement : roche, Zone prioritaire pour la biodiversité ; ou variable selon la marée : estran). La taille et la position d'une entité géographique peut être concrète (bouée, département, phare) ou floue (couloir, passe d'entrée, zone d'attente).

Un groupe d'entités géographiques est un ensemble d'un même type d'entités géographiques qui forment une ligne ou un polygone.

Une relation spatiale implique au moins deux entités pérennes du paysage hydrographique côtier.

Même si la plupart des entités pérennes du paysage hydrographique côtier figurent sur les cartes marines, il n'est pas possible d'y inclure toutes leurs propriétés. Les relations spatiales entre les entités pérennes du paysage hydrographique côtier qui figurent sur les cartes marines peuvent être déduites visuellement à partir des cartes marines.

Chaque entité pérenne du paysage hydrographique côtier est caractérisé par :

* {obligatoire} type d'entité pérenne du paysage hydrographique côtier
* {optionnel} label
* {optionnel} coordonnées géographiques
* {optionnel} relations spatiales
* {optionnel} autres entités dont elle est un élément
* {optionnel} autres entités qui la marquent
* {optionnel} hauteur (avec unités)
* {optionnel} largeur (avec unités)
* {optionnel} couleur
    * {optionnel} motif
* {optionnel} forme
* {optionnel} type de marque
    * {optionnel} type cardinal
    * {optionnel} type latéral
* {optionnel} profondeur de l'eau (avec unités)
* {optionnel} longueur verticale découverte de l'eau (avec unités)
* {optionnel} nature du fond
* {optionnel} entité géographique ou organisation qui la gère
* {optionnel} information complémentaire


**Exemple 1 :** "Vue du Nord, l’Île de Batz montre la tour du sémaphore et surtout le phare, tour grise haute de 43 m, entourée de maisons. Ce phare est équipé d’une balise d’émission AIS. L’île est débordée de tous côtés par des dangers. Les plus au large sont : à l’Est, la Basse Astan, couverte de 0,8 m d’eau, marquée par la bouée « Astan », cardinale Est lumineuse ; au Nord, la Grande Basse, couverte de 0,5 m d’eau ; à l’Ouest, Men Aodi, roche non balisée découvrant de 0,1 m."

**Exemple 2 :** "Le Canal de l’Île de Batz est un chenal profond de 0,1 à 10 m qui sépare l’Île de Batz de la côte et donne accès aux ports d’échouage de Porz Kernok (Île de Batz) et de Roscoff (§ 9.4.3.6.). On ne doit s’y engager qu’avec une bonne connaissance des lieux et le concours d’un pratique local."

**Exemple 3 :** "MOUILLAGES D’ATTENTE. — Ces mouillages, utilisés notamment par les navires se rendant à Roscoff, se trouvent dans l’Est et dans l’Ouest du chenal. Un des meilleurs se trouve au NE de la tourelle « Men Guen Bras », par profondeur de 14 m, fond de sable et coquille de bonne tenue. Prendre garde à la roche profonde de 2,8 m située à 0,3 M à l’ENE de la tourelle.
Par vents d’Est, on peut mouiller partout dans la partie Ouest du chenal jusqu’au Sud de la tourelle « Malvoch », implantée près de l’extrémité de la jetée de Porz Kernok."

**Exemple 4 :** "PORT DE L’ÎLE DE BATZ (Porz Kernok) [48° 44,6' N — 4° 00,8' W]. — Ce port d’échouage est géré par le département du Finistère. Situé sur la côte Sud de l’Île de Batz et bien protégé de tous les vents, il sert d’abri aux pêcheurs de l’île."

**Exemple 5 :** "La Pointe de Bloscon porte la chapelle de Sainte-Barbe (48° 43,6' N — 3° 58,2' W), de couleur blanche ; plus au SW on voit le clocher de Roscoff et, juste au Sud, les installations portuaires de Roscoff-Bloscon. À 3 M au SW du phare de Batz, l’Île de Siec comporte, près de son extrémité Ouest, une petite anse ouverte au Sud, protégée à l’Ouest par un môle. On peut mouiller, suivant le tirant d’eau, à l’ouvert de l’anse et dans le SW de l’extrémité Ouest de l’île, tout comme dans l’anse de Port-Neuf, située entre les communes de Cléder et Sibiril. Un mouillage pour 65 bateaux y est organisé, réglementé par l’arrêté du préfet du Finistère 20150146 - 0005 du 26 mai 2015."

**Exemple 6 :** "Moguériec (48° 41,3' N — 4° 04,3' W) est abrité au Nord par une jetée. Ce port offre un abri précaire aux pêcheurs et aux plaisanciers locaux. [...]
À l’abri de la jetée débouche un ruisseau bordé d’un quai de chaque côté. Sur la rive Nord se trouve un terre-plein et deux escaliers. Les posées, sur sable plat, sont franches partout sauf en bordure de la jetée ; les fonds découvrent de 4 à 5 m, voire de plus de 7 m à l’embouchure du ruisseau. La plupart des places à quai sont occupées par des bateaux de pêche qui y béquillent ; les bateaux de plaisance échouent entre le terre-plein et le milieu de la jetée."

**Exemple 7 :** "L’échouage de Porz Guen (48° 40,0' N — 4° 13,0' W) est protégé à l’Ouest par une digue et au Sud par un brise-lames submersible en enrochements. Il sert d’abri aux bateaux de pêche, par des fonds découvrant de 2 à 5,5 m. Le port dispose d’une cale enracinée à un terre-plein et offre une vingtaine de places sur bouées. La passe d’entrée est marquée par deux balises latérales."

**Exemple 8 :** "CHENAL DE LA MALOUINE. INSTRUCTIONS. — Ce chenal, profond de 3 m, n’a que 100 m de largeur entre le plateau de La Malouine et celui de La Pendante."

**Exemple 9 :** "9.4.5.5. Port de l’Aber-Wrac’h
L’Aber-Wrac’h (48° 35,9' N — 4° 33,7' W), établi sur la rive gauche de l’aber, entre l’Anse des Anges et l’Anse Saint-Antoine, est un port de plaisance et de pêche géré par la chambre de commerce et d’industrie de Brest.
[...]
Le mouillage de Karreg Du se trouve entre les tourelles de la Roche aux Moines et le port."

**Exemple 10 :** "Deux tourelles portant chacune un feu marquent, entre la chaussée et Guernsey, les rochers Roustel et Platte ; la première est tronconique à damier noir et blanc avec lanterne verte, la seconde est conique verte."


## Informal competency questions

**Identifiant : 1**

Question : Quels sont les caractéristiques du phare de l'Île de Batz ?

Résultat attendu : La liste des caractéristiques du phare de l'Île de Batz

Exemple : De couleur grise, haute de 43 m, équipé d’une balise d’émission AIS, entouré d'un groupe de maisons.

Dépend de : /

**Identifiant : 2**

Question : Quelle est la profondeur du Canal de l’Île de Batz ?

Résultat attendu : La liste des profondeurs du Canal de l’Île de Batz

Exemple : Profondeur de 0,1 à 10 m.

Dépend de : /

**Identifiant : 3**

Question : Où peut-on mouiller dans le chenal ?

Résultat attendu : La liste des endroits où on peut mouiller dans le chenal

Exemple : Dans l’Est du chenal, dans l’Ouest du chenal, et au NE de la tourelle « Men Guen Bras », par profondeur de 14 m, fond de sable et coquille de bonne tenue. Par vents d’Est : dans la partie Ouest du chenal jusqu’au Sud de la tourelle « Malvoch ».

Dépend de : /

**Identifiant : 4**

Question : Quelles sont les coordonnées géographiques de Porz Kernok ?

Résultat attendu : La liste des coordonnées géographiques de Porz Kernok

Exemple : Latitude 48° 41,3' N, longitude 4° 04,3' W.

Dépend de : /

**Identifiant : 5**

Question : Où se trouve le clocher de Roscoff ?

Résultat attendu : Une description de la position du clocher de Roscoff

Exemple : Au Sud-Ouest de la chapelle de Sainte-Barbe de la Pointe de Bloscon.

Dépend de : /

**Identifiant : 6**

Question : Comment peut-on stationner dans le port de Moguériec ?

Résultat attendu : Une description des possibilités pour stationner un navire dans le port de Moguériec

Exemple : Les posées, sur sable plat, sont franches partout sauf en bordure de la jetée ; les fonds découvrent de 4 à 5 m, voire de plus de 7 m à l’embouchure du ruisseau. La plupart des places à quai sont occupées par des bateaux de pêche qui y béquillent ; les bateaux de plaisance échouent entre le terre-plein et le milieu de la jetée.

Dépend de : /

**Identifiant : 7**

Question : Est-ce que Porz Guen est protégé ?

Résultat attendu : La liste des entités qui protègent Porz Guen

Exemple : À l’Ouest par une digue et au Sud par un brise-lames submersible en enrochements.

Dépend de : /

**Identifiant : 8**

Question : Quelles sont les dimensions du chenal de La Malouine ?

Résultat attendu : La liste des dimensions du chenal de La Malouine

Exemple : Profondeur de 3 m, largeur de 100 m entre le plateau de La Malouine et celui de La Pendante.

Dépend de : /

**Identifiant : 9**

Question : Où se trouve le mouillage de Karreg Du ?

Résultat attendu : La description de la position du mouillage de Karreg Du.

Exemple : Entre les tourelles de la Roche aux Moines et le port de l'Aber-Wrac'h.

Dépend de : /

**Identifiant : 10**

Question : Comment sont les rochers Roustel et Platte marquées ?

Résultat attendu : La description des entités qui marquent les rochers Roustel et Platte

Exemple : Deux tourelles portant chacune un feu, entre la chaussée et Guernsey ; la première est tronconique à damier noir et blanc avec lanterne verte, la seconde est conique verte.

Dépend de : /


## Glossaire des termes

#### Glossaire des termes

**Terme :** Entité pérenne du paysage hydrographique côtier

**Définition :** Une entité pérenne du paysage hydrographique côtier est une entité géographique ou un groupe d'entités géographiques. Les entités pérennes du paysage hydrographique côtier sont utilisées pendant une navigation pour se situer localement.

**Terme :** Entité géographique

**Définition :** Une entité géographique peut être soit naturelle (basse, fleuve, passe, raz, rive, roche, île), soit artificielle (brise-lames, cale, chapelle, clocher, digue, débarcadère, escalier, estacade, jetée, pyramide, quai, sas, sémaphore, terre-plein, tour) ou encore administrative (département, parc régional, ville) (source : https://toponymie.gouv.qc.ca/ct/normes-procedures/terminologie-geographique/entite.aspx). Une entité géographique peut être soit dans le domaine terrestre (maison, pointe, zone industriel), soit dans le domaine maritime (anse, balise, haut fond), soit les deux (invariable selon son emplacement : roche sur terre ou au large, zone prioritaire pour la biodiversité sur terre ou au large ; ou variable selon la marée : estran, roche sur le rivage). La position et la taille d'une entité géographique peut être concrète (bouée, département, phare) ou floue (couloir, passe d'entrée, zone d'attente). Une aide à la navigation peut être augmentée par une lanterne, un panneau ou un voyant.

**Terme :** Groupe d'entités géographiques

**Définition :** Un groupe d'entités géographiques est un ensemble d'un même type d'entités géographiques qui sont regroupées dans une ligne ou dans un polygone.

**Terme :** Relation spatiale

**Définition :** Une relation spatiale implique au moins deux entités pérennes du paysage hydrographique côtier. Une relation spatiale peut être concrete (la zone de mouillage est à l'Est de la jetée) ou floue (l'île est entourée de dangers). Une relation spatiale peut avoir une orientation cardinale et/ou une orientation angulaire. Une relation spatiale peut impliquer une distance entre entités. Toutes relations spatiales sont transitives (par exemple : si la bouée A est à l'Ouest de la bouée B et la bouée B est à l'Ouest de la bouée C, on peut dire que la bouée A est à l'Ouest de la bouée C) et certaines sont également inversables (par exemple : si la balise A est au Sud de la balise B, on peut dire que la balise A est au Nord de la balise B ; cependant si la tourelle C est dans l'Est de la zone D, on ne peut pas dire que la zone D est dans l'Ouest de la tourelle C).

**Terme :** Coordonnées géographiques

**Définition :** Les coordonnées géographiques d'une entité pérenne du paysage hydrographique côtier consiste de sa latitude et de sa longitude.

**Terme :** Entité marquée

**Définition :** Une entité pérenne du paysage hydrographique côtier, comme un danger, peut être marquée par une marque afin de signaler sa présence.

**Terme :** Hauteur

**Définition :** Longueur verticale de l'entité pérenne du paysage hydrographique côtier (avec unités).

**Terme :** Largeur

**Définition :** Longueur horizontale de l'entité pérenne du paysage hydrographique côtier (avec unités).

**Terme :** Élément

**Définition :** Une entité pérenne du paysage hydrographique côtier peut être composée de plusieurs éléments, qui sont également des entités pérennes du paysage hydrographique côtier, d'une façon hiérarchique. Par exemple, une île peut avoir comme élément une église, qui a elle-même comme élément un clocher. Ces relations sont obligatoirement transitives (l'île a comme élément le clocher) et inversables (le clocher est un élément de l'église, qui est elle-même un élément de l'île).

**Terme :** Couleur

**Définition :** Une entité pérenne du paysage hydrographique côtier peut être d'une ou plusieurs couleurs. Si l'entité pérenne du paysage hydrographique côtier est de plusieurs couleurs, ces couleurs peuvent être réparties selon un motif donné.

**Terme :** Motif

**Définition :** Une entité pérenne du paysage hydrographique côtier, notamment les aides à la navigation, qui est de plusieurs couleurs peut avoir ses couleurs réparties selon un motif particulier, par exemple damier, bandes horizontales, bandes verticales.

**Terme :** Forme

**Définition :** Une entité pérenne du paysage hydrographique côtier peut être d'une forme particulière, par exemple conique, rectangulaire, sphérique, tronconique.

**Terme :** Marque

**Définition :** Une marque est un type d'entité pérenne du paysage hydrographique côtier. Plus spécifiquement, une marque est un type d'aide à la navigation, généralement une balise, une bouée, un espar ou une tourelle. Une marque est une entité géographique artificielle qui est placée dans une position spécifique afin de marquer une entité pérenne du paysage hydrographique côtier ou une aide virtuelle à la navigation. Il existe cinq types de marque : les marques cardinales, les marques d'eau saine, les marques de danger isolé, les marques latérales et les marques spéciales.

**Terme :** Marque cardinale

**Définition :** Une marque cardinale comme une balise cardinale, une bouée cardinale, un espar cardinal ou une tourelle cardinale peut être placé près d'une autre entité pérenne du paysage hydrographique côtier, notamment un danger, afin de la marquer. Une marque cardinale Nord indique la présence d'un danger au Sud de la marque et qu'il faut donc passer au Nord de la marque (etc. pour les marques cardinales Est, Sud et Ouest).

Du livret Signalisation maritime du Shom :
Les marques cardinales, dont l’emploi est associé à celui du compas du navire, indiquent où le navire peut trouver des eaux saines. Elles sont partout les mêmes, quelle que soit la région, A ou B.
Une marque cardinale peut être utilisée par exemple :
* pour indiquer que les eaux les plus profondes se trouvent dans la direction (Nord, Est, Sud ou Ouest) désignée par le nom de la marque ;
* pour indiquer de quel côté d’un danger se trouvent les eaux saines ;
* pour attirer l’attention sur une configuration particulière d’un chenal telle qu’un coude, une jonction, une bifurcation ou l’extrémité d’un banc.
Les quadrants Nord, Est, Sud et Ouest sont respectivement limités par les azimuts vrais NW-NE, NE-SE, SE-SW et SW-NW dont l’origine est le point à marquer (point d’intérêt).
Une marque cardinale reçoit le nom du quadrant dans lequel elle est placée.
Le nom d’une marque cardinale indique qu’il convient de passer, par rapport à la marque, dans le quadrant qui porte ce nom.
Dans le code standard, les revêtements rétroréfléchissants des marques cardinales sont constitués d’une ou plusieurs bandes horizontales, lettres, chiffres ou symboles blancs.
Dans le code détaillé, les revêtements rétroréfléchissants des marques cardinales sont constitués comme suit :
* marques cardinales Nord : une bande horizontale bleue sur la partie noire de la marque et une bande horizontale jaune (jaune citron, d’aspect blanc de nuit lorsque éclairé par un projecteur) sur la partie jaune de la marque ;
* marques cardinales Est : deux bandes horizontales bleues sur la partie supérieure noire de la marque ;
* marques cardinales Sud : une bande horizontale jaune sur la partie jaune de la marque et une bande horizontale bleue sur la partie noire de la marque ;
* marques cardinale Ouest : deux bandes horizontales jaunes sur la partie supérieure jaune de la marque.

**Terme :** Marque d'eau saine

**Définition :** 

Du livret Signalisation maritime du Shom :
Une marque d’eaux saines indique que les eaux sont saines tout autour d’elle.
Une marque d’eaux saines sert à définir l’axe d’un chenal et le milieu du chenal. Elle peut aussi être utilisée pour indiquer un atterrissage.
Dans le code standard, les revêtements rétroréfléchissants des marques d’eaux saines sont constitués d’une ou plusieurs bandes horizontales, lettres, chiffres ou symboles, blancs ; dans le code détaillé, de paires de bandes horizontales ou verticales rouges et blanches.

**Terme :** Marque de danger isolé

**Définition :** 

Du livret Signalisation maritime du Shom :
Une marque de danger isolé indique un danger isolé d’étendue limitée autour duquel les eaux sont saines.
Dans le code standard, les revêtements rétroréfléchissants des marques de danger isolé sont constitués d’une ou plusieurs bandes horizontales, lettres, chiffres ou symboles, blancs ; dans le code détaillé, de paires de bandes horizontales bleues et rouges.

**Terme :** Marque latérale

**Définition :** 

Du livret Signalisation maritime du Shom :
Les marques latérales, dont l’emploi est associé à un « sens conventionnel de balisage », sont généralement utilisées pour des chenaux bien définis. Ces marques indiquent les côtés bâbord et tribord de la route à suivre.
Lorsqu’un chenal se divise, une marque latérale peut être utilisée pour indiquer la route qu’il convient de suivre de préférence (chenal préféré).
Les marques latérales diffèrent suivant qu’elles sont employées dans l’une ou l’autre des régions de balisage A et B.
Lorsque les marques ne sont pas identifiables d’après leur forme cylindrique ou conique, elles doivent, dans la mesure du possible, porter le voyant approprié.
Si des marques latérales de rive de chenal sont identifiées par des numéros ou des lettres, la succession des numéros (impairs à tribord et pairs à bâbord) ou des lettres suit le sens conventionnel du balisage.
Dans les codes standard et détaillé, les revêtements rétroréfléchissants des marques latérales sont constitués comme suit :
* marques latérales vertes : une bande horizontale verte ou une forme verte identique à celle du voyant ;
* marques latérales rouges : une bande horizontale rouge ou une forme rouge identique à celle du voyant.

**Terme :** Marque spéciale

**Définition :** 

Du livret Signalisation maritime du Shom :
Ces marques n’ont pas pour but principal d’aider la navigation mais elles indiquent une zone spéciale ou une configuration mentionnée dans les documents nautiques appropriés. Ce sont par exemple, des :
* marques des stations d’acquisition de données océaniques (ODAS) ;
* marques de séparation du trafic là où le balisage classique du chenal peut prêter à confusion ;
* marques indiquant les dépôts de matériaux ;
* marques indiquant des zones de pêche interdite ou de cultures marines ;
* marques indiquant des zones utilisées pour les exercices militaires ;
* marques indiquant la présence de câbles ou d’oléoducs ;
* marques indiquant des zones réservées à des activités nautiques de loisir.
Elles ne prêtent pas à confusion avec les marques donnant des informations relatives à la navigation et sont mentionnées dans les documents nautiques appropriés.
En France, les marques spéciales sont classées en deux catégories : marques durables et marques occasionnelles. Les marques spéciales durables sont surmontées d’un voyant en forme de X, jaune.
Dans les codes standard et détaillé, les revêtements rétroréfléchissants des marques spéciales sont constitués d’une bande horizontale, d’un X ou d’un symbole jaunes.

**Terme :** Direction cardinale simple

**Définition :** Nord, Est, Sud, Ouest.

**Terme :** Direction cardinale complexe

**Définition :** Nord-Est, Nord-Ouest, Sud-Est, Sud-Ouest, Nord-Nord-Est, Nord-Nord-Ouest, Sud-Sud-Est, Sud-Sud-Ouest, Est-Nord-Est, Est-Sud-Est, Ouest-Nord-Ouest, Ouest-Sud-Ouest.

**Terme :** Direction latérale

**Définition :** Bâbord (à gauche du navire), tribord (à droite du navire).

**Terme :** Organisation

**Définition :** Une organisation est une entité administrative. Elle peut être associé à un lieu donné et elle peut être cité comme gérant d'une entité géographique donnée.

**Terme :** Information complémentaire

**Définition :** Toute entité pérenne du paysage hydrographique côtier peut avoir associé à elle une information complémentaire sous la forme d'une phrase qui ne peut pas être modelé si finement.

**Terme :** Nature du fond

**Définition :** La nature du fond est une description de la nature sédimentaire du fond marin. Parfois, la qualité de la tenue du fond pour l'ancrage est également noté.

**Terme :** Profondeur de l'eau

**Définition :** La profondeur de l'eau est soit la longueur vertical d'eau entre le fond de la mer et la surface de l'eau, soit la longueur verticale d'eau au dessus d'une pérenne du paysage hydrographique côtier qui est au moins parfois submergé dans l'eau (avec unités). Cette profondeur peut être une profondeur uniforme indicative, une profondeur minimum ou une profondeur maximum.

**Terme :** Hauteur découverte de l'eau

**Définition :** La hauteur découverte de l'eau est la longueur vertical de la partie au dessus de la surface de l'eau d'une entité pérenne du paysage hydrographique côtier qui est partiellement submergé dans l'eau (avec unités).


## **Requêtes SPARQL**

**Q1 :**
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

**Q2 :**
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

**Q3 :**
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

**Q4 :**
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
Fonctionne uniquement avec inférence ?

**Q5 :**
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
Fonctionne uniquement avec inférence.

**Q6 :**
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
Comment sait-on qu'il y a une zone de stationnement dans le port pour nous expliquer le type de stationnement possible ? Ajouter un 'type de lieu de stationnement' aux ports, aux baies, etc ?

**Q7 :**
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

**Q8 :**
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
Ne fonctionne pas avec aPourDimension

**Q9 :**
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
    Fonctionne uniquement avec inference, n'est pas super clair que 'estEntre' fait référence aux deux entités ensemble -> dans le cas où une entité est entre X et Y dans une direction et entre Z et W dans une autre ?

**Q10 :**
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
Fonctionne uniquement avec inference

# GeoSPARQL

Pour créer l'index spatial :
```sparql
PREFIX geosparql: <http://www.ontotext.com/plugins/geosparql#>

INSERT DATA {
  [] geosparql:enabled "true" .
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