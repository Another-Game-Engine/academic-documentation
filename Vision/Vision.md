Page de garde
Résumé du document
Page des métadonnées
Tableau de révision

#Introduction

##Rappel de l’EIP
Epitech est une école de formation d’experts en informatique et en nouvelles technologies. L’école, membre du groupe IONIS, est répartie sur 12 sites en France. Son objectif est de former des passionnés de l’informatique à l’aide d’une pédagogie innovante axée sur les besoins réels des entreprises et sur les modes d’apprentissage de la nouvelle génération.

Outre des projets obligatoires tout au long de leur formation, les étudiants créent un projet personnel de fin d’études : l’Epitech Innovative Project (EIP). Le choix du sujet est libre, à condition que le concept de base soit innovant et techniquement intéressant. Les étudiants forment alors un groupe composé d’au minimum six élèves de leur promotion afin de réaliser leur projet de la troisième à la cinquième année. La réussite de l’EIP sera évaluée sur leurs capacités à concevoir, réaliser et présenter leur projet. Tout au long de sa réalisation, le labEIP propose de nombreux suivis afin de guider les groupes dans leur progression, et leur permettant de mener un projet dans son intégralité, avec entre autres l'intégration d’une étude de l'existant, la mise en place d’un cahier des charges, la conception, la réalisation, la communication autour du projet, l’aspect marketing, etc. Ainsi, à son terme, le projet doit être fonctionnel et en mesure d’être utilisé dans le monde professionnel.

Le but de ce travail d’innovation est de fournir aux élèves d’Epitech une pratique de gestion de projet ainsi que l’expérience d’un travail en équipe. L’ensemble donne des bases solides aux étudiants pour leur entrée dans le monde professionnel, mais aussi des ouvertures pour continuer leur projet de manière autonome.
 
## Contexte et périmètre du projet
Persuadés que l'immersion de l'utilisateur occupera une grande partie des enjeux du monde vidéo ludique de demain, nous avons décidé de créer AGE : un moteur de jeu vidéo 3D open source qui donnera une grande importance à la réalité augmentée. Ce moteur est développé en partenariat avec AMD et avec le pôle mondes virtuels du Hub innovation d’Epitech.

Nous souhaitons, à travers AGE offrir aux développeurs un outil de création de jeux vidéo exploitant les toutes dernières fonctionnalités de l’API graphique OpenGL et offrant des expériences immersives telle que de la réalité virtuelle, et en premier lieu le support de l’Oculus Rift.

## Définitions, Acronymes et Abréviations
Voici une table des définitions et acronymes, anglicismes utilisés dans ce document :
- API : une Application Programming Interface est un ensemble de classes, méthodes ou fonctions permettant d’utiliser les fonctionnalités proposées par une bibliothèque ou un service.
- Oculus Rift : un casque de réalité virtuelle, lancé en 2012 grâce à une campagne Kickstarter. Il est pour l'instant disponible uniquement dans sa version de kit de développement et est le casque de réalité virtuelle le plus attendu sur le marché de l’immersion vidéo-ludique.
- Shader : Petit programme utilisé par la carte graphique afin de générer une "frame"(voir ci-dessous). Ces shader permettent de constituer la base de l'environnement 3D d'un moteur de jeu. En effet, ce sont ce genre de programme qui applique les transformations (géométrique), les textures, ou encore les calculs de lumières essentielle au réalisme.
- Frame : Image généré par un moteur graphique. Plus le nombre de frame généré par seconde est important plus l’animation à l'écran paraitrons fluide.
- FPS : Frame Per Second indique le nombre de frame affiché par seconde. (Excellent indicateur de performance au niveau du moteur graphique)
- Moteur de jeu : Programme composé de multiple module permettant la création d'environnement virtuelle 3D ou (et) 2D (Jeux vidéo, simulateur).
- Moteur physique : module composant le "moteur de jeu" permettant la gestion de la physique dans un environnement 3D et 2D, telle que les collisions, les chutes etc.
- Moteur graphique : module composant le "moteur de jeu" permettant la gestion et la génération des éléments visibles dans une scène 3D comme 2D.
- OpenGL: API graphique permettant un contrôle sur le matériel type GPU ainsi que sur sa mémoire.
- GPU: Le Graphic Process Unit, aussi appelé carte graphique, est l'élément sur les ordinateurs utilisé pour la résolution des calculs permettant l'affichage final d'images à l'écran.
- Entity Component : 

## Références
Voici une table des références vers d’autres documents du projet et/ou sources documentaires :
Le cahier des charges V1 du projet AGE

# Besoins du projet

## Liste des besoins du projet

### L'Oculus Rift
Ce casque de réalité virtuelle est l'un besoin essentiel au projet puisqu'il permettra à AGE d'offrir aux utilisateurs de nouvelles possibilités d'interface avec les environnements générés. Il rentre dans le cadre de l'objectif d'immersion de l'utilisateur dans un environnement virtuel.

### Machines performantes

## Modules Principaux

### Le module graphique
Ce module utilisera la puissante API OpenGL afin de générer les images visibles à l'écran. Chacune de ces images sera le fruit d'une accumulation d'effet dit "Shader" qui seront traiter et optimisé au travers d'une "pipeline" conçu par nos soin. De plus, Ce module aura pour objectif de partager un maximum de tâche par le GPU par l'intermédiaire d'OpenGL, afin que celui-ci prenne en charge les calculs redondant (calcule matricielle, interpolation). Par ce biais nous espérons pouvoir traité un grand nombre d'élément dans nos scène tous en garantissant des performances (nombre de FPS) acceptables.

### Le moteur physique
Il s'agit du module responsable de la gestion des interactions entre les divers objets 3D de nos scènes ainsi que de la gravité. Pour ce faire, nous utiliserons la technologie libre "Bullet", puissante et stable déjà présente sur des produits notable telle que Blender.

### Le Core
Considéré comme le cœur du moteur de jeu, il s'agit du module responsable de la logique. Il orchestre l'ensemble des autres modules dans une architecture cohérente, maintenable et optimisé. Sur AGE, le core présente un modèle de type "Entity Component", ceci afin de garantir une flexibilité dans son utilisation et son développement.

# Produit et Solution

## Architecture logique
Vous présenterez dans cette section, l’architecture logique (grands building blocs) de votre projet avec les modules principaux.
Faire un petit UML de component

## Flux et interactions

### Flux d’activité
Faire un bon UML d’activité

### Interactions avec l'extérieur (OS, Périphériques, etc)
Faire un petit UML de déploiement

### Interactions utilisateurs 
Améliorer mon UML Cas d’utilisation

# Choix des technologies

## Infrastructure

## Composants logiciels

Nous utilisons dans notre moteur de jeu plusieurs bibliothèques externes.

Tout d'abord, pour la gestion de la physique, nous avons choisi d'utiliser Bullet.
Voici une matrice de comparaison des différents moteurs physiques existants permettant de comparer leurs avantages et inconvénients:

Nom                      Plateformes                        Licence        GPU / CPU          Puissance

Nvidia PhysX             Consoles, Windows, Linux           Propriétaire   GPU et CPU         Très perfomant
Newton Game Dynamics     Windows, Mac, IOS, Linux           Open Source    CPU (GPU en Beta)  Moyennement performant
Open Dynamics Engine     Windows, Mac, Linux                Open Source    CPU                Moyennement performant
Tokamak                  Windows, Mac, Linux                Open Source    CPU                Moyennement performant
Bullet                   PS3, Windows, Mac, Linux           Open Source    CPU et GPU         Très performant

Bullet s'impose comme la référence des moteurs physiques open source, étant à la fois extrèmement performant et précis, mais permettant aussi une flexibilité que ne permettent pas les autres (il est possible de remplacer chaque partie de la bibliothèque pour pouvoir coder ses propres comportements par exemple).

Nous avons ensuite du choisir une bibliothèque nous permettant de charger nos objets 3D. En effet, il est important de pouvoir travailler avec des graphistes pendant la conception d'un projet, et il est donc nécessaire de pouvoir charger facilement des formats de fichiers permettant de décrire des objets, des scènes, des animations et des matériaux facilement. Voici la matrice de comparaison des différents SDK permettant le chargement de ce genre de fichiers:

Nom             Licence        Format(s)         Supporte

Open Collada    Open source    .dae              Modèles, Animations, Lumières, Caméras, Matériaux
Blitz3D SDK     Open source    .b3d              Modèles, Animations, Matériaux
Fbx SDK         Propriétaire   .fbx, .dae, .obj  Modèles, Animations, Lumières, Caméras, Matériaux

Comme vous pouvez le voir, le Fbx SDK développé par Autodesk permet le chargement de tous les types de fichier les plus utilisés par les infographistes 3D sans contraintes d'exportation (pas de plugin à installer sur les Blender ou 3dsmax par exemple). Notre choix c'est donc orienté vers cette bibliothèque.

Il était aussi important de choisir un outils permettant de sérialiser facilement des scènes de notre moteur de jeu, de facon à pouvoir les recharger facilement. Le but était donc de trouver une bibliothèque rapide et permettant l'export en différents types de formats (en ASCII pour pouvoir éditer les fichiers à la main facilement et en binaire pour gagner du temps de chargement). Voici le tableau permettant de comparer les différentes bibliothèques existantes:

Nom            Langage    Licence       ASCII / Binaire    Format                Taille de la bibliothèque

Boost          C++        Open source   ASCII et Binaire   Xml, Custom, Binaire  Très importante
libs JSon      C / C++    Open source   ASCII              Json                  Très faible
libs Xml       C / C++    Open source   ASCII              Xml                   Très faible
protobuf       C++        Open source   Binaire            Binaire               Faible
Cereal         C++11      Open source   ASCII et Binaire   Xml, Json, Binaire    Moyenne

Nous avons donc choisi "cereal" car il s'agit de la librairie nous offrant la plus grande flexibilité quand au formats d'écriture en plus d'être assez légère. De plus, étant codé en C++11, elle offre des facilités syntaxiques que les autres ne peuvent proposer.

Enfin, il était important de choisir une bibliothèque permettant de lire du son, ce qui est essentiel dans un moteur de jeu. Pour cela, nous avons du choisir entre ces différents composants:

Nom           Plateformes                     Licence        Prix      Haut / Bas niveau       Son 3D

PortAudio     Windows, Mac, Linux             Open source    Gratuit   Bas niveau              Non
OpenAL        Windows, Mac, Linux             Open source    Gratuit   Haut niveau             Oui
SDL Mixer     Windows, Mac, Linux             Open source    Gratuit   Bas niveau              Oui
FMOD          Windows, Mac, Linux, consoles   Propriétaire   Payant    Haut niveau             Oui

Nous nous sommes finalement orienté vers FMOD car ... bah je sais pas pourquoi en fait, OpenAL à l'air cool quand même :P

 
## Multi OS

Notre projet consistant principalement à exploiter la technologie OpenGL 4, nous ne pourrons pas nous rendre compatible avec les systèmes d'eploitation autres que Windows.
En effet, les drivers des cartes graphiques sur Linux ne supportent pas cette version d'OpenGL.
Pour autant, le reste de notre moteur sera entièrement portable car nous avons choisis uniquement des bibliothèques et technologies multi-plateforme

__________________________________________________________________
| Technologie         |    Plateforme(s) supportée(s)            |
|_____________________|__________________________________________|
| Moteur de jeu:                                                 |
|----------------------------------------------------------------| 
| C++ 11 (et STL)          Windows, Linux, Mac                   |
| Cereal                   Windows, Linux, Mac                   |
| Bullet                   Windows, Linux, Mac, Consoles de jeux |
| FMOD                     Windows, Linux, Mac, Consoles de jeux |
| OpenGL 4                 Windows                               |
|________________________________________________________________|
| Outils:                                                        |
|----------------------------------------------------------------|
| Qt                       Windows, Linux, Mac                   |
| FBXsdk                   Windows, Linux, Mac                   |
|________________________________________________________________|

Nous esperons donc pouvoir, dès la sortie des drivers adéquats sur Linux, pouvoir rendre notre produit multi OS.

# Synthèse budgétaire

## L’Oculus Rift
L’équipe de développement d’AGE disposera dans peu de temps de son propre Oculus Rift, commandé au cours du mois d’avril 2014, avec les moyens de l’équipe. Cependant, les deux membres de l’équipe s’occupant de l’intégration de l’Oculus Rift ne poursuivront pas leur quatrième année dans le même pays, soit :
 - César Leblic (leblic_c) sera à Concordia (Canada) de mois année à mois année.
 - Anthony Boucher (bouche_t) quant à lui passera son année à San Marco (Etats-Unis) de mois année à mois année.
Puisque César à payé la totalité du matériel, nous avons convenus qu’il conserverait l’Oculus Rift avec lui lors de son année à l’étranger. Mais nous souhaitons disposer d’un second Oculus Rift le temps de 12 mois pour Anthony Boucher, 4 mois lors du début de sa quatrième année en France et 8 mois lors de son année aux États-Unis.

Le prix d’un Oculus Rift est de : 350 dollars.

## Ressources 3D
Au cours du développement d’AGE, des tests seront effectués afin de valider l’utilisabilité et la performance du moteur de jeu. Les démonstrations qui résulteront de ces tests serviront également à présenter notre produit et à communiquer autour de lui.
L’équipe a donc besoin d’une bibliothèque de ressources 3D élaborées, constitué de modéle 3D ainsi que des textures associé (bump map, normal map, diffuse map).

Nous avons estimés le prix de ces ressources 3D à : nbr euros.

## Salons

## Résumé des coûts


