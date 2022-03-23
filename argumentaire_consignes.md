### Modelet : Consignes de navigation et règlements

#### Scénario de motivation

**Nom :** Consignes de navigation et règlements

**Dernière mise à jour :** 21 juillet 2021

**ID entités géographiques :** (ent:6000)

**Description :** Les _Instructions Nautiques_  contiennent des consignes de navigation et des règlements. Les consignes de navigation indiquent les manières de naviguer et les moyens de stationner dans une zone côtière donnée afin de garantir la sûreté de toutes et de tous. Une consigne de navigation peut être une information, une instruction, une interdiction ou un renseignement lié à la navigation ou au stationnement d'un navire. Les règlements indiquent les noms d'arrêtés qui s'appliquent dans des cas spécifiques dans le domaine maritime. Les interdictions citent toujours un ou des règlements et les informations en font référence parfois.

Une information peut stipuler un avis ou une recommendation sur la navigation, le stationnement ou toute autre action possible dans le domaine maritime, ou bien un avis à caractère administratif. Une information est liée à un ou des lieux d'effet, ou implique une ou des entités géographiques. Une information peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une information peut être imposée par un règlement.

Une instruction concerne soit l'action de naviguer, soit l'action de stationner, soit l'action d'attendre. Une instruction peut donc détailler soit la manière conseillée de naviguer d'un point de départ donné à un point de destination donné, soit le ou les lieux de stationnement conseillés dans un contexte donné, soit les consignes pour les zones d'attentes. Une instruction de navigation indique la ou les aides virtuelles à la navigation à suivre, dans un ordre donné. Une aide virtuelle à la navigation peut être un alignement, un dispositif de séparation du trafic (DST), un relèvement, un repérage, une route ou un secteur. Une instruction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une instruction peut faire référence à une information.

Une interdiction détaille une ou des actions interdites dans un lieu donné. Une interdiction est liée à un ou des lieux d'effet. Une interdiction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une interdiction est imposée par un règlement.

Un renseignement donne les coordonnées d'un contact donné dans un port. Un contact peut avoir un numéro de téléphone, un chenal VHF et une adresse mail. Aux numéros de téléphone et aux chenaux VHF peuvent être associées des horaires. La ville dans laquelle se trouve le port est le lieu d'effet du renseignement.

Un règlement donne le code, la date et l'auteur de l'arrêté cité.

La description des consignes de navigation est souvent caractérisée par des actions : **laisser** à bâbord (resp. tribord), **laisser** Platte Fougère et Petite Canupe respectivement à 0,7 et 0,5 M (distance) dans l’Ouest (orientation), **suivre** l'alignement ou le relèvement, **suivre** l’axe du secteur blanc (253° – 255°) du feu de la jetée Nord, **suivre** ce chenal, **éviter** le 1,6 m découvrant de la roche Colombier à 0,4 M du Pont de la Gaîne, Le Chenal du Bunel permet **d’éviter** le Chenal de la Petite Porte, il est **interdit** de mouiller dans un cercle de 0,25 M de rayon centré sur le point situé à 085° et 460 m du phare de White Rock Pier.

Toutes ces informations ne figurent pas sur les cartes marines et sont recherchées par les navigateurs dans les IN lorsqu'ils préparent leur mission.

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


**Exemple 1 :** "En venant de l’Est, on prend le chenal en suivant l’alignement à 293,3° du clocher de l’Île de Batz (chapelle Notre-Dame de Bon Secours), sur la côte Sud de l’île, par la pyramide blanche de l’Île Pigued (48° 44,0' N — 3° 58,2' W). Cet alignement n’est visible par les petits navires que jusqu’à environ 0,6 M à l’Est de la tourelle « Le Menk » (à mi-marée) et, par les navires à passerelle plus haute, jusqu’au Nord de la tourelle ; il se situe dans le secteur blanc (289,5° – 293°) du feu de la tourelle « Ar Chaden » (§ 9.3.3.1.). La route à 293,3° laisse au Nord le Plateau des Duons et au Sud Bazenn ar Menk (tourelle « Le Menk », cardinale Ouest lumineuse), et la Basse de Bloscon (bouée cardinale Nord lumineuse). Les petits navires d’où il n’est pas possible de voir le clocher de l’Île de Batz, masqué par la végétation, peuvent se présenter légèrement à gauche de l’alignement de garde à 290° du phare de l’Île de Batz par la tourelle « Ar Chaden »."

**Exemple 2 :** "Les navires qui se dirigent de La Manche vers Gibraltar et l’Atlantique, ou inversement, peuvent soit passer très au large d’Ouessant, soit emprunter le dispositif de séparation du trafic d’Ouessant ou, s’ils remplissent les conditions voulues (§ 2.3.4.2.), suivre la route côtière à l’Ouest d’Ouessant, ou bien encore emprunter le Chenal du Four au Nord et le Raz de Sein au Sud."

**Exemple 3 :** "De nuit, la Grande Passe ne peut être pratiquée que s’il fait assez clair pour distinguer les tourelles et les bouées proches du chenal."

**Exemple 4 :** "La pratique des véhicules nautiques à moteur dans l’archipel de Molène au sein du parc naturel marin d’Iroise est interdite, à l’exception de l’accès à l’île Molène par le chenal des Laz, dans un couloir de 300 m de largeur centré sur l’alignement au 264°, conformément à l’arrêté 2014/32 du 10 juin 2014 du préfet maritime de l’Atlantique (disposible sur le site www.premar-atlantique.gouv.fr/arretes.html)."

**Exemple 5 :** "RÉSERVE NATURELLE (arrêté 78/94 du 4 avril 1978 du maire de Granville). — Les îles et îlots situés à l’Est de la ligne joignant le phare de Grande Île à la tourelle « L’Enseigne » constituent une réserve ornithologique. Leur accès est interdit du 1er avril au 30 juin. L’île Aneret (ou Grande Ancre) n’est pas concernée par cette interdiction. Le mouillage des navires de plaisance est interdit du 1er avril au 31 juillet dans une zone, portée sur la carte, aux abords de l’îlot des Guernesiais (48° 53,7' N — 1° 48,7' W)"

**Exemple 6 :** "ZONE INTERDITE DE LA CENTRALE DE GRAVELINES (arrêté 17/2010 du 3 mai 2010 du préfet maritime de La Manche et de la Mer du Nord). — La navigation, le mouillage, le dragage, le stationnement, la pêche à partir d’embarcation, la baignade, la plongée sous-marine, le dépôt sur le fond de la mer de tout engin lourd ou toute autre activité maritime sont interdits aux abords du centre nucléaire de production d’électricité de Gravelines dans une zone, portée sur les cartes, située immédiatement à l’Ouest du Port Ouest de Dunkerque."

**Exemple 7 :** "Les chenaux d’accès et la zone d’attente du STM de Dunkerque sont intégrés à la partie maritime de la Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque, créée par l’arrêté interpréfectoral 45/2014 du 18 juillet 2014 du préfet maritime de la Manche et de la mer du Nord et du préfet du Nord (disponible sur le site www.premar-manche.gouv.fr)."

**Exemple 8 :** "Les navires de plaisance en attente d’entrée dans le Vieux Bassin sont tenus de stationner à la Jetée de la Lieutenance et au Quai du Jardin Public (partie matérialisée par des flèches blanches)."

**Exemple 9 :** "4.5.5.5. Saint-Valéry-sur-Somme
\[...]
RENSEIGNEMENTS. — Département de la Somme (80) ; 2 700 habitants.
Bureau du port et maison des plaisanciers : au port de plaisance ; tél. : 03.22.60.24.80 ; VHF ; saison de 07 h 00 à 23 h 00 (en fonction des heures de marées), hors-saison : de 09 h 00 à 12 h 00 et de 14 h 00 à 17 h 00 ; mél. : snval@wanadoo.fr.
Gendarmerie maritime : tél. : 03.22.60.82.08.
Sas : tél. : 03.22.60.80.23."

**Exemple 10 :** "6.2.2.4. Courseulles-sur-Mer
\[...]
RENSEIGNEMENTS. — Département du Calvados (14) ; 4 200 habitants.
Bureau du port : Quai Ouest du Bassin Joinville ; tél. : 02.31.37.51.69 (de – 3 PM à + 3 PM) ; VHF (heures ouvrables).
Douanes : au bureau du port.
Vigie, cabine de l’écluse : tél. : 02.31.37.46.03."

**Exemple 11 :** "INSTRUCTIONS. — Le navire venant du large, après avoir reconnu la bouée d’atterrissage « Le Légué », doit donner un large tour vers l’Est à la bouée « 1 » afin de parer le Banc de la Toupie. Il navigue ensuite entre les bouées du chenal pour se présenter sensiblement dans l’axe du sas de l’écluse. Par mauvais temps de NE, il est conseillé aux navires sans pilote de rester aux abords de la bouée d’atterrissage."

**Exemple 12 :** "Fécamp ( 49° 53,3' N — 0° 41,8' E) est un port de pêche, de commerce et de plaisance. C’est un port départemental géré par la chambre de commerce et d’industrie de Fécamp-Bolbec.
\[...]
Il est recommandé d’entrer à la fin du courant de flot et peu de temps avant l’heure de la pleine mer qui est aussi l’heure de l’étale. L’heure favorable d’entrée d’un gros navire est en général, une demi-heure avant la pleine mer (une heure avant par gros temps de NE).
L’entrée ne comporte pas de méthode a priori, si ce n’est d’approcher en se maintenant sur l’alignement à 082° (§ 4.8.2.), jusqu’à quelques centaines de mètres de la Jetée Sud puis d’utiliser la forte dérive due au courant, la barre, la machine en avant, pour parer aussi près que possible le musoir de la Jetée Sud.
À ce moment il faut demeurer particulièrement attentif aux embardées du navire notamment lorsque l’avant commence à se trouver à l’abri du courant. Par forte houle d’Ouest, la tenue du cap peut ainsi devenir trop difficile pour permettre l’entrée."

**Exemple 13 :** "À marée basse et par beau temps calme, il est possible, pour un navire de plaisance ou une embarcation, d’accoster le socle de cette balise [la balise « Jet d’Amont »]."

#### Informal competency questions

**Identifiant : 1**

Question: Comment peut-on accéder au chenal 4011 ? Idem si on navigue dans un petit navire ?

Résultat attendu: La liste des consignes de navigation pour accéder au chenal 4011 ; idem pour un petit navire.

Exemple: En venant de l’Est, on prend le chenal en suivant l’alignement à 293,3° du clocher de l’Île de Batz (chapelle Notre-Dame de Bon Secours), sur la côte Sud de l’île, par la pyramide blanche de l’Île Pigued (48° 44,0' N — 3° 58,2' W). Cet alignement se situe dans le secteur blanc (289,5° – 293°) du feu de la tourelle « Ar Chaden » (§ 9.3.3.1.). La route à 293,3° laisse au Nord le Plateau des Duons et au Sud Bazenn ar Menk (tourelle « Le Menk », cardinale Ouest lumineuse), et la Basse de Bloscon (bouée cardinale Nord lumineuse). Les petits navires peuvent se présenter à 290° du phare de l’Île de Batz par la tourelle « Ar Chaden ».

Dépend de: /

**Identifiant : 2**

Question: Quelles sont les itinéraires possibles pour se diriger de La Manche vers Gibraltar ?

Résultat attendu : La liste des aides virtuelles à la navigation à suivre afin d'accéder à Gibraltar depuis La Manche.

Exemple: Soit passer très au large d’Ouessant, soit emprunter le dispositif de séparation du trafic d’Ouessant ou, si les conditions XYZ sont remplies, suivre la route côtière à l’Ouest d’Ouessant, ou bien encore emprunter le Chenal du Four au Nord et le Raz de Sein au Sud.

Dépend de: /

**Identifiant : 3**

Question: Peut-on pratiquer la Grande Passe de nuit ?

Résultat attendu: Les consignes concernant la pratique de la Grande Passe de nuit.

Exemple: De nuit, la Grande Passe ne peut être pratiquée que s’il fait assez clair pour distinguer les tourelles et les bouées proches du chenal.

Dépend de: /

**Identifiant : 4**

Question : Y a-t-il des interdictions au sein du parc naturel marin d’Iroise ?

Résultat attendu: La liste des interdictions au sein du parc naturel marin d'Iroise, l'arrêté associé et, au cas échéant, le cible de l'interdiction et ses exceptions.

Exemple: La pratique des véhicules nautiques à moteur dans l’archipel de Molène au sein du parc naturel marin d’Iroise est interdite, à l’exception de l’accès à l’île Molène par le chenal des Laz, dans un couloir de 300 m de largeur centré sur l’alignement au 264°, conformément à l’arrêté 2014/32 du 10 juin 2014 du préfet maritime de l’Atlantique (disposible sur le site www.premar-atlantique.gouv.fr/arretes.html).

Dépend de: /

**Identifiant : 5***

Question : Quand peut-on mouiller dans la zone 6032 ?

Résultat attendu : La liste de toutes les conditions permettant de mouiller dans la zone 6032.

Exemple : Le mouillage des navires de plaisance est interdit du 1er avril au 31 juillet dans une zone, portée sur la carte, aux abords de l’îlot des Guernesiais (48° 53,7' N — 1° 48,7' W).

Dépend de: /

**Identifiant : 6**

Question : Où est située la zone interdire de la centrale de Gravelines ?

Résultat attendu : La description de la positionnement de la zone interdire de la centrale de Gravelines.

Exemple : Aux abords du centre nucléaire de production d’électricité de Gravelines dans une zone, portée sur les cartes, située immédiatement à l’Ouest du Port Ouest de Dunkerque.

**Identifiant : 7**

Question : Quel arrêté est à l'origine de la Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque ?

Résultat attendu : Les informations concernant l'arrêté à l'origine de la Zone Maritime et Fluviale de Régulation (ZMFR) du port de Dunkerque.

Exemple : L’arrêté interpréfectoral 45/2014 du 18 juillet 2014 du préfet maritime de la Manche et de la mer du Nord et du préfet du Nord (disponible sur le site www.premar-manche.gouv.fr).

**Identifiant : 8**

Question : Quels sont les consignes pour entrer dans le Vieux Bassin ?

Résultat attendu : La liste des consignes pour entrer dans le Vieux Bassin.

Exemple : Les navires de plaisance en attente d’entrée dans le Vieux Bassin sont tenus de stationner à la Jetée de la Lieutenance et au Quai du Jardin Public (partie matérialisée par des flèches blanches).

**Identifiant : 9**

Question : Comment puis-je contacter le Bureau du port à Saint-Valéry-sur-Somme ?

Résultat attendu : La liste des coordonnées du Bureau du port à Saint-Valéry-sur-Somme.

Exemple : Bureau du port et maison des plaisanciers : au port de plaisance ; tél. : 03.22.60.24.80 ; VHF ; saison de 07 h 00 à 23 h 00 (en fonction des heures de marées), hors-saison : de 09 h 00 à 12 h 00 et de 14 h 00 à 17 h 00 ; mél. : snval@wanadoo.fr.

**Identifiant : 10**

Question : Qui peut-on contacter à Courseulles-sur-Mer ? Quels sont leurs numéros de téléphone ? Y a-t-il des horaires associées aux numéros de téléphone ?

Résultat attendu : La liste des contacts à Courseulles-sur-Mer et, si disponibles, leurs numéros de téléphone et les horaires des numéros.

Exemple : Bureau du port : Quai Ouest du Bassin Joinville, 02.31.37.51.69, de – 3 PM à + 3 PM. Douanes : au bureau du port. Vigie, cabine de l’écluse, 02.31.37.46.03.

Dépend de : /

**Identifiant : 11**

Question : Comment entrer dans le sas de l'écluse 6059 ?

Résultat attendu : La liste des consignes pour entrer dans l'écluse 6059.

Exemple : Le navire venant du large, après avoir reconnu la bouée d’atterrissage « Le Légué », doit donner un large tour vers l’Est à la bouée « 1 » afin de parer le Banc de la Toupie. Il navigue ensuite entre les bouées du chenal pour se présenter sensiblement dans l’axe du sas de l’écluse. Par mauvais temps de NE, il est conseillé aux navires sans pilote de rester aux abords de la bouée d’atterrissage.

**Identifiant : 12**

Question : Où est localisé le port de Fécamp ?

Résultat attendu : Les coordonnées géographiques du port de Fécamp ou une description de ses relations spatiales.

Exemple : 49° 53,3' N — 0° 41,8' E

**Identifiant : 13**

Question : Est-ce qu'il est possible d'accoster la balise « Jet d’Amont » ?

Résultat attendu : La liste des conditions qui permettent l'accostage de la balise « Jet d’Amont ».

Exemple : À marée basse et par beau temps calme, il est possible, pour un navire de plaisance ou une embarcation, d’accoster le socle de la balise « Jet d’Amont ».


#### Glossaire des termes

**Terme :** Consigne de navigation

**Définition :** Les consignes de navigation indiquent les manières de naviguer et les moyens de stationner dans une zone côtière donnée afin de garantir la sûreté de toutes et de tous. Une consigne de navigation peut être une information, une instruction, une interdiction ou un renseignement lié à la navigation ou au stationnement d'un navire.

**Terme :** Cap

**Définition :** Un cap désigne l'orientation du navire exprimée en degrés (voir thèse Wissame, p.46).

**Terme :** Instruction

**Définition :** Une instruction est une consigne de navigation. Une instruction concerne soit l'action de naviguer, soit l'action de stationner. Une instruction peut donc détailler soit la manière conseillée de naviguer d'un point de départ donné à un point de destination donné, soit le ou les lieux de stationnement conseillés dans un contexte donné. Une instruction implique de suivre une séquence d'aides à la navigation. Une instruction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une instruction peut faire référence à une information.

**Terme :** Alignement

**Définition :** Un alignement est une aide virtuelle à la navigation. Un alignement peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction. Un alignement est un concept qui aligne au moins deux repères, ce qui représente une ligne qui forme un angle avec le nord (voir thèse Wissame, p.47). Cet angle est le cap. Le premier repère cité est celui le plus loin du navire.

**Terme :** Relèvement

**Définition :** Un relèvement correspond à une orientation sur un repère, ce qui définit un angle formé entre ce repère et la direction du nord géographique à partir du navire (voir thèse Wissame, p.47). Cet angle est le cap. Un relèvement est une aide virtuelle à la navigation. Un relèvement peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction.

**Terme:** Interdiction

**Définition :** Une interdiction est une consigne de navigation. Les interdictions citent toujours un ou des règlements et les informations en font référence parfois. Une interdiction détaille une ou des actions interdites dans un lieu donné. Une interdiction est liée à un ou des lieux d'effet. Une interdiction peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une interdiction est imposée par un règlement.

**Terme :** Règlement

**Définition :** Les règlements indiquent les noms d'arrêtés qui s'appliquent dans des cas spécifiques dans le domaine maritime. Un règlement donne le code, la date et l'auteur de l'arrêté cité.

**Terme :** Information

**Définition :** Une information est une consigne de navigation. Une information peut stipuler un avis ou une recommendation sur la navigation, le stationnement ou toute autre action possible dans le domaine maritime, ou bien un avis à caractère administratif. Une information est liée à un ou des lieux d'effet, ou implique une ou des entités géographiques. Une information peut avoir une cible, peut dépendre de la temporalité, des conditions météorologiques ou des conditions océanographiques, et peut avoir des exceptions. Une information peut être imposée par un règlement.

**Terme :** Renseignement

**Définition :** Un renseignement est une consigne de navigation. Un renseignement donne les coordonnées d'un contact donné dans un port. Un contact peut avoir un numéro de téléphone, un chenal VHF et une adresse mail. Aux numéros de téléphone et aux chenaux VHF peuvent être associées des horaires. La ville dans laquelle se trouve le port est le lieu d'effet du renseignement.

**Terme:** Route

**Définition:** Une route peut être, mais n'est pas limitée à, une route côtière connue (par exemple : "route côtière à l'Ouest d'Ouessant"), un chenal, une description d'un itinéraire (par exemple : "donner un large tour vers l'Est à la bouée « 1 »"), une ligne définie par un point de départ et un point de destination. Une route est une aide virtuelle à la navigation. Une route peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction.

**Terme:** Secteur

**Définition:** Un feu à secteurs est un [balisage](https://fr.wikipedia.org/wiki/Balisage "Balisage") lumineux ([phare](https://fr.wikipedia.org/wiki/Phare "Phare") ou feu) qui est utilisé pour guider de nuit les navires dans un [chenal](https://fr.wikipedia.org/wiki/Chenal_maritime "Chenal maritime") cerné de dangers (écueils, absence de fonds). La couleur du feu perçue par l'observateur situé sur le navire varie en fonction de l'[azimut](https://fr.wikipedia.org/wiki/Azimut "Azimut") du signal lumineux et permet au navigateur de savoir s'il se trouve placé correctement dans le chenal. Le feu à secteurs comporte généralement un secteur lumineux blanc qui désigne la zone libre de dangers et des secteurs lumineux rouge et vert qui désignent les secteurs dangereux (rouge à [bâbord](https://fr.wikipedia.org/wiki/B%C3%A2bord "Bâbord") de la zone saine, vert à [tribord](https://fr.wikipedia.org/wiki/Tribord "Tribord")). Si le bateau s'écarte de la zone des eaux saines, le signal lumineux devient selon le cas rouge ou vert permettant d'effectuer la correction dans la bonne direction. Le feu à secteurs est une alternative à un balisage plus couteux consistant à placer des bouées lumineuses tout au long du chenal. Dans certains lieux de navigation ([chenal](https://fr.wikipedia.org/wiki/Chenal "Chenal") non rectiligne, ...), le navire doit parfois suivre successivement plusieurs feux à secteur. (Source : https://fr.wikipedia.org/wiki/Feu_%C3%A0_secteurs). Un secteur est une aide virtuelle à la navigation. Un secteur peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction.

**Terme :** Dispositif de séparation du trafic (DST)

**Définition :** Un dispositif de séparation de trafic comprend généralement deux voies de circulation séparées par une zone de séparation de trafic ; il peut contenir également des zones de changement de route (rond-point) orientant les navires vers d'autres voies secondaires. Le DST peut être matérialisé par le [balisage](https://fr.wikipedia.org/wiki/Balisage "Balisage") (bouées ou [phares](https://fr.wikipedia.org/wiki/Phare "Phare")), mais aujourd'hui tenant compte des possibilités de [positionnement par satellites](https://fr.wikipedia.org/wiki/Navigation_par_satellite), les DST qui visent à éloigner le trafic des côtes sont « virtuels », et définis par les seules positions des sommets des zones de réglementation, et par les règles de navigation dans ces zones. (Source : https://fr.wikipedia.org/wiki/Dispositif_de_s%C3%A9paration_du_trafic). Un DST est une aide virtuelle à la navigation. Un DST peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction.

**Terme :** Repérage

**Définition :** Un repérage consiste à reconnaître un repère, ce qui permet de se situer localement. Un repérage est une aide virtuelle à la navigation. Un repérage peut faire partie d'une séquence d'aides virtuelles à la navigations à suivre, elle-même impliquée dans une instruction. Par exemple : "après avoir reconnu la bouée d’atterrissage « Le Légué »".

**Terme :** Aide virtuelle à la navigation

**Définition :** Une aide virtuelle à la navigation peut être un alignement, un dispositif de séparation du trafic (DST), un relèvement, un repérage, une route ou un secteur. Une instruction implique de suivre une séquence d'aides à la navigation.

**Terme :** Action

**Définition :** Une action correspond à une activité maritime. Une action peut être, mais n'est pas limitée à, la baignade, le dragage, le dépôt sur le fond de la mer de tout engin lourd, la navigation, la plongée sous marine, la pêche à partir d'embarcation ou le stationnement.

**Terme :** Cible

**Définition :** Le cible d'une information, d'une instruction ou d'une interdiction désigne le type de navire ou le ou les caractéristiques qu'un navire doit avoir pour être concerné par la consigne de navigation. Si une consigne de navigation n'a pas de cible, tous types de navires sont concernés.

**Terme :** Condition météorologique

**Définition :** Toute information, instruction ou interdiction peut dépendre des conditions météorologiques. Une condition météorologique peut désigner n'importe quel phénomène météorologique, ainsi que la direction et la puissance qui lui sont associées.

**Terme :** Condition locale

**Définition :** Toute information, instruction ou interdiction peut dépendre des conditions locales : la temporalité, les conditions météorologiques ou les conditions océanographiques.

**Terme :** Condition océanographique

**Définition :** Toute information, instruction ou interdiction peut dépendre des conditions océanographiques. Une condition océanographique peut être un courant (d'un type, d'une direction ou d'une force donnés) ou un état de la marée (haute, basse, montante, descendante, de vives-eaux, de mortes-eaux). Une condition océanographique peut aussi faire référence à une temporalité (30 minutes avant ou après la pleine mer).

**Terme :** Temporalité

**Définition :** Toute information, instruction ou interdiction peut dépendre de la temporalité. La temporalité peut être qualitative ou quantitative, et peut désigner des horaires, une période de la journée (le jour, la nuit, avant le coucheur du soleil), des dates, des mois ou des saisons.

**Terme :** Lieu d'effet

**Définition :** Une consigne de navigation peut être associée à un lieu d'effet. Ce lieu est l'endroit où la consigne prend effet.s

#### **Requêtes SPARQL**

**Q1 :**
Comment peut-on accéder au chenal 4011 ? (ent:4011 parce qu'il s'agit d'une entité non-nommé)
Pour avoir les alignements possibles  :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
SELECT DISTINCT ?cible ?pointDeDepart ?aideVirtuelleALaNavigation ?typeDAideVirtuelleALaNavigation
WHERE {
?ent rdf:type nav:Instruction.
?ent nav:aPourAction tac:Navigation.
?ent nav:aPourPointDeDestination ent:4011.
?ent nav:aPourPointDeDepart ?pointDeDepart.
?ent nav:impliqueDeSuivre ?nb.
?nb ?label ?aideVirtuelleALaNavigation.
    FILTER (strstarts(str(?label), str(rdf:_)))
?aideVirtuelleALaNavigation a ?typeDAideVirtuelleALaNavigation.
    OPTIONAL {?ent nav:aPourCible ?cible}
}
```
Comment peut-on accéder au chenal 4011 si on navigue dans un petit navire ?
Pour avoir les alignements possibles pour un petit navire :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tta: <http://data.shom.fr/id/codes/nav/typedetaille/>
SELECT DISTINCT ?cible ?pointDeDepart ?aideVirtuelleALaNavigation ?typeDAideVirtuelleALaNavigation
WHERE {
?ent rdf:type nav:Instruction.
?ent nav:aPourAction tac:Navigation.
?ent nav:aPourPointDeDestination ent:4011.
?ent nav:aPourPointDeDepart ?pointDeDepart.
?ent nav:impliqueDeSuivre ?nb.
?nb ?label ?aideVirtuelleALaNavigation.
    FILTER (strstarts(str(?label), str(rdf:_)))
?aideVirtuelleALaNavigation a ?typeDAideVirtuelleALaNavigation.
?ent nav:aPourCible ?cible.
?cible a nav:Navire.
?cible nav:aPourTaille tta:Petit.
}
```

**Q2 :**
Quelles sont les itinéraires possibles pour se diriger de La Manche vers Gibraltar ?
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
SELECT DISTINCT ?type ?itineraire
WHERE {
?ent rdf:type nav:Instruction.
?ent nav:aPourPointDeDepart/rdfs:label "La Manche"@fr.
?ent nav:aPourPointDeDestination ?destination.
?destination ?label1 ?ent2.
    FILTER (strstarts(str(?label1), str(rdf:_)))
?ent2 rdfs:label "Gibraltar"@fr.
?ent nav:impliqueDeSuivre ?selection.
?selection ?label2 ?ent3.
    FILTER (strstarts(str(?label2), str(rdf:_)))
?ent3 rdfs:label ?itineraire.
?ent3 a ?type.
}
```
Avec rdf:member ; fonctionne uniquement avec inference (https://stackoverflow.com/questions/16121150/sparql-query-rdf-container-rdf-bag/16130842) :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
SELECT DISTINCT ?ent ?qqch ?s ?nom
WHERE {
?ent nav:aPourPointDeDepart ent:6013.
    ?ent nav:aPourPointDeDestination ?destination.
?destination ?label1 ?ent2.
    FILTER (strstarts(str(?label1), str(rdf:_)))
?ent2 rdfs:label "Gibraltar"@fr.
?ent nav:impliqueDeSuivre ?qqch.
?qqch rdf:member ?s.
?s rdfs:label ?nom
}
```

**Q3 :**
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

**Q4 :**
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

**Q5 :**
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

**Q6 :**
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

**Q7 :**
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

**Q8 :**
Quels sont les consignes pour entrer dans le Vieux Bassin ?
Pour avoir toutes les informations sur naviguer jusqu'au Vieux Bassin :
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
SELECT DISTINCT ?propriete ?info
WHERE {
?ent nav:aPourPointDeDestination ?pointDeDestination.
?pointDeDestination rdfs:label "Vieux Bassin"@fr.
?ent ?propriete ?info.
}
```

**Q9 :**
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

**Q10 :**
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

**Q11 :**
Comment entrer dans le sas de l'écluse 6059 ?
```sparql
PREFIX nav: <http://data.shom.fr/def/navigation_cotiere#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX teg:<http://data.shom.fr/id/codes/nav/typedentitegeographique/>
PREFIX ent: <http://data.shom.fr/id/entitegeographique/>
PREFIX rlsp: <http://data.shom.fr/def/relationsspatiales#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>
PREFIX tna: <http://data.shom.fr/id/codes/nav/typedenavire/>
PREFIX tac: <http://data.shom.fr/id/codes/nav/typedaction/>
SELECT DISTINCT ?cible ?ordre ?typeDAideVirtuelleALaNavigation ?nom
WHERE {
?ent nav:aPourPointDeDestination ent:6059.
?ent nav:impliqueDeSuivre ?nb.
?nb ?ordre ?aideVirtuelleALaNavigation.
    FILTER (strstarts(str(?ordre), str(rdf:_)))
?aideVirtuelleALaNavigation a ?typeDAideVirtuelleALaNavigation.
?aideVirtuelleALaNavigation rdfs:label ?nom.
    OPTIONAL {?ent nav:aPourCible ?cible}}
```

**Q12 :**
Où est localisé le port de Fécamp ?
Pour avoir les coordonnées géographiques et/ou les relations spatiales autour du port de Fécamp :
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
SELECT DISTINCT ?ent ?cdg ?rlsp ?propriete
WHERE {
?ent rdfs:label "Fécamp"@fr.
?ent nav:aPourNature teg:Port.
	OPTIONAL {?ent nav:aPourCoordonneesGeographiques ?cdg.
        ?ent ?propriete ?cdg}
    OPTIONAL {?ent nav:aUneRelationSpatialeAvec ?rlsp.
        ?ent ?propriete2 ?rlsp}
}
```
Fonctionne uniquement avec inférence

**Q13 :**
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

# GeoSPARQL

Pour créer l'index spatial :
```sparql
PREFIX geosparql: <http://www.ontotext.com/plugins/geosparql#>

INSERT DATA {
  [] geosparql:enabled "true" .
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