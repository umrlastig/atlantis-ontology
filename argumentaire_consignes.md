# Argumentaire du modelet Consignes

## Nom
Consignes de navigation et règlements

## Description
Les _Instructions Nautiques_  contiennent des consignes de navigation et des règlements. Les consignes de navigation indiquent les manières de naviguer et les moyens de stationner dans l'environnement maritime côtier. Une consigne de navigation peut être une information, une instruction, une interdiction ou un renseignement lié à la navigation ou au stationnement d'un navire. Les règlements indiquent les noms d'arrêtés qui s'appliquent dans des cas spécifiques dans le domaine maritime. Les interdictions citent toujours un ou des règlements et les informations en font référence parfois.

Une information peut stipuler un avis ou une recommendation sur la navigation, le stationnement ou toute autre action possible dans le domaine maritime, ou bien un avis à caractère administratif. Une information est liée à un ou des lieux d'effet, ou implique une ou des entités géographiques. Une information peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une information peut être imposée par un règlement.

Une instruction concerne soit l'action de naviguer, soit l'action de stationner, soit l'action d'attendre. Une instruction peut donc détailler soit la manière conseillée de naviguer d'un point de départ donné à un point de destination donné, soit le ou les lieux de stationnement conseillés dans un contexte donné, soit les consignes pour les zones d'attentes. Une instruction de navigation indique la ou les aides virtuelles à la navigation à suivre, dans un ordre donné. Une aide virtuelle à la navigation peut être un alignement, un dispositif de séparation du trafic (DST), un relèvement, un repérage, une route ou un secteur. Une instruction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une instruction peut faire référence à une information.

Une interdiction détaille une ou des actions interdites dans un lieu donné. Une interdiction est liée à un ou des lieux d'effet. Une interdiction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une interdiction est imposée par un règlement.

Un renseignement donne les coordonnées d'un contact donné dans un port. Un contact peut avoir un numéro de téléphone, un chenal VHF et une adresse mail. Aux numéros de téléphone et aux chenaux VHF peuvent être associées des horaires. La ville dans laquelle se trouve le port est le lieu d'effet du renseignement.

Un règlement donne le code, la date et l'auteur de l'arrêté cité.

La description d'une consigne de navigation ou d'un règlement est caractérisé par :
* {information, instruction, interdiction, renseignement : obligatoire} type de consigne de navigation
* {information, interdiction, renseignement : obligatoire} entité(s) impliquée(s) dans/lieu d'effet de la consigne de navigation
* {instruction, interdiction : obligatoire} action à réaliser/action interdite selon la consigne de navigation
* {instruction : obligatoire} Features à suivre selon l'instruction
* {information : obligatoire} stipulation donne par l'information
* {règlement : obligatoire} arrêté à l'origine du règlement
* {information, instruction, interdiction, renseignement : optionnel} règlement à l'origine de la consigne de navigation
* {information, instruction, interdiction, renseignement : optionnel} cible de la consigne de navigation
* {information, instruction, interdiction : optionnel} condition locale sous laquelle la consigne de navigation est valide
    * {information, instruction, interdiction : optionnel} temporalité de la consigne de navigation (de nuit, entre 10h00 et 17h00, en été)
    * {information, instruction, interdiction : optionnel} condition météorologique sur laquelle la consigne de navigation dépende (par vents de ouest)
    * {information, instruction, interdiction : optionnel} condition océanographique sur laquelle la consigne de navigation dépende  (à marée basse, à vives-eaux)
* {information, instruction, interdiction : optionnel} exception à la consigne de navigation
* {instruction : optionnel} information complémentaire à l'instruction

## Exemples
### Exemple 1
"En venant de l’Est, on prend le chenal en suivant l’alignement à 293,3° du clocher de l’Île de Batz (chapelle Notre-Dame de Bon Secours), sur la côte Sud de l’île, par la pyramide blanche de l’Île Pigued (48° 44,0' N — 3° 58,2' W). Cet alignement n’est visible par les petits navires que jusqu’à environ 0,6 M à l’Est de la tourelle « Le Menk » (à mi-marée) et, par les navires à passerelle plus haute, jusqu’au Nord de la tourelle ; il se situe dans le secteur blanc (289,5° – 293°) du feu de la tourelle « Ar Chaden » (§ 9.3.3.1.). La route à 293,3° laisse au Nord le Plateau des Duons et au Sud Bazenn ar Menk (tourelle « Le Menk », cardinale Ouest lumineuse), et la Basse de Bloscon (bouée cardinale Nord lumineuse). Les petits navires d’où il n’est pas possible de voir le clocher de l’Île de Batz, masqué par la végétation, peuvent se présenter légèrement à gauche de l’alignement de garde à 290° du phare de l’Île de Batz par la tourelle « Ar Chaden »." [C2A, p. 529]

### Exemple 2
"Les navires qui se dirigent de La Manche vers Gibraltar et l’Atlantique, ou inversement, peuvent soit passer très au large d’Ouessant, soit emprunter le dispositif de séparation du trafic d’Ouessant ou, s’ils remplissent les conditions voulues (§ 2.3.4.2.), suivre la route côtière à l’Ouest d’Ouessant, ou bien encore emprunter le Chenal du Four au Nord et le Raz de Sein au Sud." [C22, p. 428-429]

### Exemple 3
"De nuit, la Grande Passe ne peut être pratiquée que s’il fait assez clair pour distinguer les tourelles et les bouées proches du chenal." [C22, p. 351]

### Exemple 4
"La pratique des véhicules nautiques à moteur dans l’archipel de Molène au sein du parc naturel marin d’Iroise est interdite, à l’exception de l’accès à l’île Molène par le chenal des Laz, dans un couloir de 300 m de largeur centré sur l’alignement au 264°, conformément à l’arrêté 2014/32 du 10 juin 2014 du préfet maritime de l’Atlantique (disposible sur le site www.premar-atlantique.gouv.fr/arretes.html)." [C22, p. 434, 451]

### Exemple 5
"RÉSERVE NATURELLE (arrêté 78/94 du 4 avril 1978 du maire de Granville). — Les îles et îlots situés à l’Est de la ligne joignant le phare de Grande Île à la tourelle « L’Enseigne » constituent une réserve ornithologique. Leur accès est interdit du 1er avril au 30 juin. L’île Aneret (ou Grande Ancre) n’est pas concernée par cette interdiction. Le mouillage des navires de plaisance est interdit du 1er avril au 31 juillet dans une zone, portée sur la carte, aux abords de l’îlot des Guernesiais (48° 53,7' N — 1° 48,7' W)" [C2A, p. 422]

### Exemple 6
"ZONE INTERDITE DE LA CENTRALE DE GRAVELINES (arrêté 17/2010 du 3 mai 2010 du préfet maritime de La Manche et de la Mer du Nord). — La navigation, le mouillage, le dragage, le stationnement, la pêche à partir d’embarcation, la baignade, la plongée sous-marine, le dépôt sur le fond de la mer de tout engin lourd ou toute autre activité maritime sont interdits aux abords du centre nucléaire de production d’électricité de Gravelines dans une zone, portée sur les cartes, située immédiatement à l’Ouest du Port Ouest de Dunkerque." [C2A, p. 138]

### Exemple 7
"Les chenaux d’accès et la zone d’attente du STM de Dunkerque sont intégrés à la partie maritime de la Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque, créée par l’arrêté interpréfectoral 45/2014 du 18 juillet 2014 du préfet maritime de la Manche et de la mer du Nord et du préfet du Nord (disponible sur le site www.premar-manche.gouv.fr)." [C2A, p. 139]

### Exemple 8
"Les navires de plaisance en attente d’entrée dans le Vieux Bassin sont tenus de stationner à la Jetée de la Lieutenance et au Quai du Jardin Public (partie matérialisée par des flèches blanches)." [C2A, p. 290]

### Exemple 9
"4.5.5.5. Saint-Valéry-sur-Somme
\[...]
RENSEIGNEMENTS. — Département de la Somme (80) ; 2 700 habitants.
Bureau du port et maison des plaisanciers : au port de plaisance ; tél. : 03.22.60.24.80 ; VHF ; saison de 07 h 00 à 23 h 00 (en fonction des heures de marées), hors-saison : de 09 h 00 à 12 h 00 et de 14 h 00 à 17 h 00 ; mél. : snval@wanadoo.fr.
Gendarmerie maritime : tél. : 03.22.60.82.08.
Sas : tél. : 03.22.60.80.23." [C2A, p. 204-205]

### Exemple 10
"6.2.2.4. Courseulles-sur-Mer
\[...]
RENSEIGNEMENTS. — Département du Calvados (14) ; 4 200 habitants.
Bureau du port : Quai Ouest du Bassin Joinville ; tél. : 02.31.37.51.69 (de – 3 PM à + 3 PM) ; VHF (heures ouvrables).
Douanes : au bureau du port.
Vigie, cabine de l’écluse : tél. : 02.31.37.46.03." [C2A, p. 306, 308]

### Exemple 11
"INSTRUCTIONS. — Le navire venant du large, après avoir reconnu la bouée d’atterrissage « Le Légué », doit donner un large tour vers l’Est à la bouée « 1 » afin de parer le Banc de la Toupie. Il navigue ensuite entre les bouées du chenal pour se présenter sensiblement dans l’axe du sas de l’écluse. Par mauvais temps de NE, il est conseillé aux navires sans pilote de rester aux abords de la bouée d’atterrissage." [C22, p. 303]

### Exemple 12
"Fécamp ( 49° 53,3' N — 0° 41,8' E) est un port de pêche, de commerce et de plaisance. C’est un port départemental géré par la chambre de commerce et d’industrie de Fécamp-Bolbec.
\[...]
Il est recommandé d’entrer à la fin du courant de flot et peu de temps avant l’heure de la pleine mer qui est aussi l’heure de l’étale. L’heure favorable d’entrée d’un gros navire est en général, une demi-heure avant la pleine mer (une heure avant par gros temps de NE).
L’entrée ne comporte pas de méthode a priori, si ce n’est d’approcher en se maintenant sur l’alignement à 082° (§ 4.8.2.), jusqu’à quelques centaines de mètres de la Jetée Sud puis d’utiliser la forte dérive due au courant, la barre, la machine en avant, pour parer aussi près que possible le musoir de la Jetée Sud.
À ce moment il faut demeurer particulièrement attentif aux embardées du navire notamment lorsque l’avant commence à se trouver à l’abri du courant. Par forte houle d’Ouest, la tenue du cap peut ainsi devenir trop difficile pour permettre l’entrée." [C2A, p. 224, 226]

### Exemple 13
"À marée basse et par beau temps calme, il est possible, pour un navire de plaisance ou une embarcation, d’accoster le socle de cette balise [la balise « Jet d’Amont »]." [C2A, p. 341]