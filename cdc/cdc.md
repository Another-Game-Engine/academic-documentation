# Resume du document

Ce document contient la liste des besoins, des exigences et des contraintes qu'il faudra respecter lors de la réalisation du projet AGE. Il servira à donner une ligne de conduite à l’équipe de réalisation qui devra suivre son contenu.
Le projet est d'abord décrit dans ton ensemble, puis nous exposons leur objectifs, les cibles visées sont ensuite citées, ainsi que les outils utilisés au cours du developpement. La description des différentes parties du programme montre ensuite de manière plus approfondie le travail qui sera effectué. 

Pour finir, on listera les différents outils qui permettront à l’équipe d’avoir une organisation optimale.

# Rappel de l’EIP 

## Objectifs de l’EIP et Epitech 

### Presentation d'Epitech

Fondée en 1999, Epitech est une école d'informatique proposant aux étudiants une pédagogie innovante. Cette dernière, axée sur la pratique, cherche à former des individus autonomes, à travers la réalisation de projets concrets.

Ces travaux permettent aux étudiants de se confronter à des problématiques techniques, méthodologiques et organisationnelles :

- Techniques, car ces projets requièrent certaines notions et compétences pour être réalisés.
- Méthodologiques, car ces notions ne sont pas encore connues de l’étudiant, il devra donc s'adapter aux problèmes afin d’y trouver des solutions.
- Organisationnels, car les étudiants doivent gérer leur temps de travail, leur planning ainsi que leurs différents groupes de projets.

### Presentation de l'EIP

L’Epitech Innovative Project est un projet de groupe, de la troisième à la cinquième année, permettant de valider le master de l’Epitech.

Les étudiants sont chargés de se réunir en groupe. Le choix du projet est libre - ils ont la possibilité de reprendre un projet existant ou de développer une idée innovante. La réussite de l’EIP sera évaluée sur leurs capacité à concevoir, réaliser et présenter leur projet. Tout au long de sa réalisation, de nombreux suivis ont lieu, permettant de guider les groupes dans leur progression.

Le but de l’EIP est de permettre aux étudiants de mener un projet dans son intégralité : étude de l'existant, mise en place d’un cahier des charges, conception, réalisation, communication, marketing etc.

A son terme, le projet doit être fonctionnel et en mesure d’être utilisé dans le monde professionnel.

Le laboratoire EIP propose des cours de communication ainsi que des suivis de groupe et de projets, permettant de suivre les avancées du projet ainsi que sa gestion.

## Presentation de AGE

### Presentation du produit

AGE est un moteur de jeu video 3D open source, exploitant les dernières fonctionnalités du langage C++ et de l’Application Programming Interface (API) graphique OpenGL.

Nous souhaitons, à travers AGE offrir aux développeurs un outil de création de jeux vidéo et d'expérience immersive (réalité virtuelle).

### Les objectifs techniques

Les caractéristiques majeures d'AGE peuvent être réunies sous les points suivants :
- Flexibilité
- Performance
- Innovations graphiques

#### Moteur flexible et complet

AGE propose une architecture extrêmement modulable, basée sur le système Entity Component System permettant d'accueillir tout type de jeux vidéo. Effectivement, cette architecture, de plus en plus présente dans les moteurs de jeux modernes, permet au game engine d’accueillir un large éventail de gameplay différents.

En effet, son coeur a été pensé pour permettre un large éventail d'utilisation.
De plus, il mettra à la disposition des utilisateurs une série d'outils facilitant le développement de contenus vidéoludiques de haute qualité (éditeur de scène 3D, éditeur de modèle 3D, ...).

Plus encore, il sera compatible avec l'Occulus Rift (casque de réalité augmentée), de manière native et sans développements supplémentaires.

Pour finir, AGE comprendra en son sein une série de fonctionnalités indispensables au développement de jeux vidéo et d'expériences immersives - tels qu'un moteur physique et des effets graphiques avancés.

#### Performance

AGE est un moteur de jeu pensé pour apporter de très grandes performances.

En effet les technologies qu'il utilise ont été sélectionnées pour leur modernité et leur efficacité.

Ainsi, son coeur sera développé en C++11 (puis porté en C++14 lorsque les compilateurs atteindront leur maturité).

L'architecture a été pensée pour épouser au mieux les dernières configurations matérielles des ordinateurs (calcul GPU, multithreading, x64).

#### Graphismes modernes

AGE se propose d'être un outil innovant graphiquement dans le domaine de l'open source, et plus largement, dans l'industrie du jeu vidéo et de la réalité augmentée. En effet, AGE a été pensé pour utiliser les dernières versions de l'API graphique OpenGL (4.3 - 4.4), nous permettant de bénéficier au maximum des derniers pilotes Nvidia et AMD.

De plus, AGE proposera une technique de rendu 3D très rare, le tile forward rendering. Cette méthode, extrêmement récente - et dont beaucoup d'experts s'accordent à qualifier de très prometteuse - n'est pour le moment que très peu présente dans le secteur vidéoludique.

AGE comprendra en son sein, une méthode de rendu graphique flexible et moderne, en plus de divers effets de qualités, ce qui permettra à l'utilisateur d'ajouter dans son produit, une importante quantité de source de lumière et d'ombres tout en conservant de bonnes performances.

### Les objectifs sur le marche

#### Immersion et realite virtuelle

Persuadés que l'immersion de l'utilisateur occupera une grande partie des enjeux du monde vidéoludique de demain, nous avons décidé de donner une grande importance à la réalité augmentée, et en premier lieu, à l'Oculus Rift.

De plus, nous procéderons à une intégration complète du moteur physique open source Bullet, pour permettre aux développeurs de proposer une physique riche et réaliste aux utilisateurs.

#### Open Source

// TODO ! TROUVER UNE LICENCE

AGE est un moteur 3D open source dont le code est disponible à tous pour consultation, édition et utilisation.
Il est aujourd'hui accessible sur GitHub en dépo public à l'adresse : https://github.com/Another-Game-Engine/AGE

Ceci est possible en grande partie par le choix des technologies utilisé : OpenGL, Bullet, GLM, Cereal, etc (technologies gratuites et ouvertes).

### Les cibles

#### Utilisateurs potentiels

es principaux utilisateurs ciblés par notre moteur sont d'une part les entreprises.

En effet, aujourd'hui la scène française du jeu vidéo n'est pas homogène en termes de techniques utilisées.
D'une part, les grands acteurs (Ubisoft, Eugen Software, Quantic Dream) développent des moteurs performants en interne et de manière propriétaire ; d'autre part les plus petites sociétés ont recourt à des solutions open source peu chères, ne réunissant jamais flexibilité, performance et rendu graphique.

C'est dans un tel contexte qu'AGE prend son sens, en offrant aux entreprises un moteur open source comprenant les dernières fonctionnalités en termes de jeux vidéo 3D.

Ce constat est le même pour la scène de la réalité virtuelle et de l'éducation, le domaine ayant connu une récente explosion venant entre autres de l'évolution des technologies et des matériels (Oculus Rift, Google Glass, Kinect ...).
Ce domaine a besoin de nouveau outils qui lui permettraient de se développer encore plus vite.
Nous voulons donc développer notre moteur en forte collaboration avec des acteurs présents dans le monde de la réalité augmentée.

Nous aurons l'occasion d'approfondir cette étude dans la suite du document.

#### Les profils techniques cibles

AGE a pour objectif d'apporter aux développeurs un moteur de jeu alliant grande flexibilité de développement, hautes performances et grande qualité graphique.
C'est pourquoi ce projet open source est à destination des développeurs confirmés, maîtrisant le C++ à un niveau avancé.
Néanmoins, il est prévu d’y intégrer une documentation complète ainsi que de nombreux exemples permettant à des développeurs moins expérimentés de tenter leur chance.

#### Les plateformes ciblees

AGE est conçu dans un premier temps pour être compatible avec la plateforme Windows. En effet, seule cette dernière permet aujourd’hui l'utilisation des dernières fonctionnalités OpenGL.
Cependant, afin de permettre au plus grand nombre d’utiliser notre moteur dans leur environnement de travail, nous espérons développer la compatibilité Mac et Linux (sous réserve que les derniers pilotes graphiques soient disponible sur le système d’exploitation).

# Présentation de l’environnement de réalisation 

## Environnement de réalisation 

### Langages et API utilisees

#### C++11

AGE est developpe en C++11, nouvelle norme pour le langage C++.

Cette version offre au moteur et a ses utilisateurs une plus grande flexibilite de developpement grace de nombreuses nouvelles fonctionnalités tout facilitant le developpement pour les débutants.

Parmis les nombreuses nouvelles fonctionnalités, ceux qui nous interessent particulièrement sont ceux permettant d'augmenter la rapidé du code (std::move, std::forward, ...) ainsi que les outils permettant de se passer au maximum de librairire exterieurs. En effet, dans ce nouveau standard, on été implémenté des fonctionnalités concernant l'interopérabilité des systèmes tel que les threads. Notre moteur ayant pour but d'être particulierement performant, ce fut un point important de notre choix vers cette technologie.

#### OpenGL 4.3

Les versions openGL 4.x nous permettent de tirer profit des formidables ressources des GPU modernes. 

Les versions openGL 4.x nous permettent de tirer profit des formidables ressources des GPU modernes.
En effet un grand nombre de nouvelles fonctionnalités favorisent l'utilisation de la VRAM (mémoire interne au GPU) afin que les données soient plus aisément accessible par la carte graphique.
De plus certaines de ses fonctionnalités - telles que le "compute" OpenGL - permettent de supplanter certaines librairies comme OpenCL en matière d'utilisation GPU.

Ainsi AGE a pour ambition de suivre l'exceptionnel croissance du marché du calcul massivement parallèles. Grace au soutien du constructeur AMD nous avons la possibilité d'avoir des retours sur l'utilisation de ce matériel de plus en plus puissant et prometteur.

#### GLSL 

GLSL est un langage permettant l'écriture de shaders, nous l'utilisons aujourd'hui dans sa version 400.

AGE a pour objectif de déporter un maximum de ses calculs en GLSL dans des shaders, afin de les paralléliser au maximum sur le GPU pour un traitement plus rapide.

// à améliorer

### Plateformes et outils de developpement

#### Windows x64

AGE est developpe sur Windows 8.1, dans sa version 64 bits.

En effet, les derniers pilotes graphiques sont developpes pour la plateforme Windows 8.
De plus, AGE etant pense pour etre utilise sur une architecture 64 bits (il sera tout de meme compatible avec les architecture 32 bits), il est necessaire de disposer d'un environnement de developpement 64 bits.

#### Visual studio 2013

AGE est developpe a l'aide de l'IDE (Integrated Development Environment) Visual Studio. Nous utilisons la derniere version de celui-ci (2013) car elle apporte de nombreuse fonctionnalites indispensable au projet AGE.
En effet, celle-ci, en plus d'offrir de nouveaux outils de debugging, supporte la compilation du C++11 essentielle au fronctionnement du moteur de jeux.

#### CodeXL

Nous utilisons CodeXL, un outil de debugging sur GPU gratuit, developpe et maintenu par l'entreprise AMD.

Ce logiciel offre beaucoup de fonctionnalites essentielles au developpement sur carte graphique, parmis lesquels :
- Detection des erreurs OpenGL
- Break points
- Edit and continue sur les shaders
- Inspection des FBO et des VBO au runtime

#### Git

Git est un outils de versionning, specifiquement concu pour faciliter d'une part la sauvegarde de l'historique de production, et d'autre part, la collaboration entre developpeurs sur un meme projet.

// TODO : Descrtiption des fonctionnalites de Git

## Environnement matériel 

### Environnement de developpement

#### Ordinateur moderne

AGE etant destine aux architectures materieles modernes, il est necessaire pour son developpement de travailler sur un ordinateur recent.
Par consequenent, la majorite des developpeurs d'AGE disposent d'un ordinateur reunissant :
- Un processeur multicoeur (Intel I5 / I7) accelerant le temps de compilation.
- Un disque dur SSD approtant a Visual Studio 2013 un meilleur temps de reponse pour l'autocompletion.
- Une carte graphique recente et puissante permettant le calcul GPU et l'affichage d'effets complexes a l'ecran.

#### Oculus Rift

L'Oculus Rift etant integre au projet, il nous est necessaire de disposer d'un Oculus pour le developpement d'AGE. Par consquent, nous avons commande un kit de developpement Oculus, et sommes en attente de sa livraison.

L'Oculus que nous allons utiliser sera le dernier prototype (Mars 2014). Cela nous permettra d'integrer a AGE les dernieres fonctionnalites offertent par le produit.

#### Periqueriques de controle

##### Xbox Controller

De maniere a augmenter l'immersion des joueurs, AGE integrera le support de la manette Xbox. Par consequent l'equipe de developpement du moteur a en sa possession plusieurs des ces produits.

##### Razer hydra (on le tente ou pas ?)

##### STEM System (on le tente ou pas ?)
// http://www.sixensestore.com/stemsystem-2.aspx

### Environnement de production

C'est le meme environnement que l'environnement de developpement

Vous présenterez dans cette partie le matériel nécessaire à la réalisation et au déploiement de 
votre projet (depuis l’environnement de développement à l’environnement de production). 

## Architecture technique 

### Le moteur de jeux

#### L'architecture Entity Component System

##### Les entites

- Memory friendly (avoid cash miss)
- Octree
- Graphnode

##### Les composants

- Memory friendly (avoid cash miss)

##### Les systemes

- Updated in different threads

##### Les prefabs

##### Les filtres

- Update unsecrure thread
- Update secured thread
- Memory pool for entity holders

#### Chargement et sauvegarde

##### Load and save threaded

##### Multi format
- XML, JSON, Binary

##### Threaded streaming d'entite

#### La gestion de la physique

##### Integration des rigid bodys

##### Integration des joints

##### Integration des softbody

##### Integration des breakable body

##### Callback de collision / information de collision

##### HotZones

##### Character controller

##### Box2D

##### Demembration / Mutilation dynamique

##### Ragdoll

##### Interfacage pour multi lib

#### Gameplay

##### NavMesh

#### La gestion des assets

##### Les Textures

##### Les mesh de rendu

##### Les animations

##### Les materials

##### Les sprites

##### Les polices

##### Les modeles de collisions

##### Les modeles de "friction / bounciness ..."

##### Level of details (simplification de mesh)

#### Le son

##### Son 3D avec FMOD

##### Sound emitter / Sound reciever

##### Reverb

##### Interfacage pour multi libs

##### Sound culling (blocage du son sur obstacle)

#### GUI

- Textarea
- Textinput
- Buttons (hover, mousedown, mouseup)
- Slider range
- Checkbox
- Radio buttons

##### 2D GUI

##### 3D GUI

#### Utils

##### Tweening

##### Bezier path

##### Random

##### Hashmaps

##### Custom RTTI

##### Configuration manager

##### Evaluation du hardware et configuration des options en fonction de celui-ci

##### Interfacage des inputs

#### Benchmark

- Scene vertices count
- Culled vertices count
- FPS
- Rendering time
- Update time
- Total CPU time
- Entity count
- Effect count
- Particle count
- Decal count
- Rigid body count
- Light count
- Update time persystem

### Le moteur graphique

#### High Dynamic Range (HDR)

le HDR est un post effet permettant de simuler et cela dynamiquement, le fonctionnement de la rétine lors d'un éblouissement.

#### Dynamic Shadow Mapping

Technique permettant la mise en place d'ombre réaliste calculer dynamiquement.

#### Reflection Mapping

Effet utilisant le sampler opengl "Cube Map" afin de simuler le visuel d'un miroir et cela de manière sphérique.

#### Anti-Aliasing

Afin de réduire le crénelage dans nos rendu, nous appliquerons l'algorithme FXAA permettant de diminuer drastiquement la pixelisations des bords de nos géométries.

#### Tile Base rendering

Le "tile based light culling" est une méthode de "culling" des lumières permettant de ne calculer l'influence des lumières uniquement sur les zones de l'écran influencées par celles-ci.
Ainsi, si une scène à un grand nombre de lumières dynamiques, nous n'allons pas calculer l'illumination que chaqu'une d'entres elles provoque sur chaque pixel de notre écran, mais juste celles qui influencent réellement la zone de l'écran dans laquelle se situe le pixel.

##### deffered rendering

Nous allons coupler la technique du "tile based rendering" avec une méthode de rendu appellée "Deffered rendering" et permettant le calcul des lumières uniquement sur les "fragment" réellement affichée.
Ainsi, si un fragment passe le test du light culling mais ne fait pas partie du rendu final, car il est par exemple caché par une géometrie qui s'affichera par dessus, les influences des différentes lumières ne seront pas calculées pour celui-ci.
Cet effet permet aussi la mise en place de nombreux algorithme, comme par exemple de la global illumination.

##### foward rendering

Nous proposerons aussi une méthode de rendu "classique", permettant notemment de rendre des objets semi-transparents dans nos scenes.
Cette méthode va juste rendre tous les objets de la scene, sans tenir compte du fait qu'il soit cachés par quelconque géometrie.

#### Decals

#### Dynamic skybox

#### Architecture

##### Command list
- Draw commands organized in a parallel thread

#### Particles

- GPU based
- Vector fields
- Interactive

### Les outils d'editions

#### Editeur de niveau
-> Edition de prefab
-> Creation de scene
-> Placement des entity et prefabs
-> Configuration des systems dans les scene
-> Configuration des des entity et components
-> Pixel picker for selection of objects

#### Convertisseur d'assets

##### Gestion de la bibliotheque
-> Serialisation Obj, Fbx, Tga, Mtl, Jpg, Png, Bullet, Fonts
-> Edition Obj, Fbx, Mtl
-> Generation des collider physiques

##### Previsualisation

-> Material, Mesh, Textures
-> Physique

Listez ici les systèmes, le stockage de données, et autres composants de votre solution. Vous devez 
également décrire globalement les interactions et dépendances entre les grands composants de 
votre solution, mais aussi votre mécanisme de staging. 

## Composants existants 

### Technologies integrees au moteur

##### SDL

La SDL est une bibliothéque graphique multiplate-forme libre est totalement gratuite sur ça version 1.x. Son utilisation dans notre moteur est principalement : la création de fenêtre et la gestion des événements clavier/souris.

##### Bullet

Bullet est un moteur physique permettant la gestion des interactions entre divers corps dans un environement 3D.
Il comprend dans ses nombreuses fonctionnalitées :
- Collisions
- Rigidbody
- Culling d'objet
- // Cesar complète ou corrige :)
Tout comme la SDL il est sous licence zlib et alloue à ses utilisateurs une utilisation libre.


##### FBX SDK

Kit de dévellopement permettant le chargement de modèle FBX. Le modèles FBX est un format de fichiers contenant toutes les informations nécessaire à la réalisation d'objet 3D. Il comprend :
- géométrie
- couleur
- normal
- texture
- animation
- ect...
Développé par autodesk il fait partie aujourd'hui des formats les plus utilisé au monde par les graphistes et animateur 3D.

##### Cereal

// Cesar 

##### Oculus SDK

L'oculus rift est un casque/lunnette de réalité augementé à destination du grand public. Cette outils se prèsente comme le périphèrique centrale de notre objectif d'immersivité. Ayant pour charge de renforcer l'expérience de l'utilisateur dans le virtuelle, l'oculus rift sera l'occasion pour AGE de mettre en valeur c'est effet graphique et physique d'une façon innovante et bien plus immersive.

##### FMOD

// ça serait bien de pas en parler

##### GLM

GLM est une libraire de mathématique quasiment integré à openGL. Elle nous permet d'effectuer tout nos calcules matricielle et contenir la plus part de nos donnée scalaire (position, normal, couleur ect).

##### FreeType

// Cesar

### Technologies de gestion de projet

#### Github

##### Issues - Milestones

Afin de favoriser la communication durant le développement, nous utiliserons le système d'issue et de Milestones proposé par GitHub. Chaque nouvelle implémentation, mise à jour ou débogage seront précédés par une issue assigné au membre de l'équipe concernée. Ceci permettra une bonne visibilité sur la totalité des tâches à abattre ainsi que de leur réalisation.

Les Milestones permettront de placer ces issues dans un contexte de temps afin d'imposer des échéances au diverses parties du projet.

##### Pull request

Chaque nouvelle fonctionnalité majeure devra être validé par l'ensemble du groupe avant d'être mergé au coeur du projet, ceci afin de garantir la stabilité du code finale.
Pour ce faire nous utiliserons le système de pull request et de branche offert par github.
La base du projet sera sur la branche dite "master".
Le reste du développement se fera sur des branches parallèles.

##### Wiki

Le Wiki comprendra deux genres de documentation:
- D'abord, un plan détaillé de l'architecture du moteur ainsi que de ses diverses fonctionnalités et de leur utilisation. Cette documentation a pour objectif d'aider les utilisateurs potentiels à prendre en main le moteur de jeu.
- ensuite une documentation aux objectifs plus axé "recherche et développement", qui décrira le fonctionnement certaine implémentation plus complexe comme par exemple "Tile Foward rendering". Afin de pouvoir soumettre aux interressés un retour d'expérience sur les problèmes rencontrés, les solutions apportés et le résultat obtenus.

#### Google Mailing List

Afin de communiquer efficacement par mail, nous avons mis en place grâce aux outils googles une mailling list baptisé Ageproject.

La quasi totalité de notre communication interne se fera soit par cette ML, soit par Hang Out.

Vous décrirez ici les cas de réutilisation des composants déjà existants sur lesquels vous vous 
basez, leurs caractéristiques principales, leur cycle de vie et leur dépendance à votre projet. 


## Gestion de la sécurité 

Vous décrirez comment vous gérez la sécurité, techniques et outils. 
f. Points sensibles 
Vous listerez ici les risques sur le projet, qui devront faire l’objet de suivi et d’attention sur le 
projet, et vous proposerez un plan d’action si le risque se produit. 

# Description des différentes parties du programme à réaliser 

Vous présenterez l’architecture générale du programme, les fonctionnalités du projet, les interactions 
entre les composants fonctionnels, les programmes et fonctionnalités que vous aurez en résultat. Vous 
organiserez cette partie en fonction de votre sujet et domaine. 

# Description des tests de premier niveau 

Vous décrirez les plans de tests, outils utilisés pour la réalisation des tests. 

# Organisation projet 

Vous décrirez votre organisation projet en termes de ressources, planning et méthodologie 

# Annexes
