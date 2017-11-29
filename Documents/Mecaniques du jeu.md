# Mécaniques du jeu
# Général

## Progression du jeu

La progression dans le jeu se fait par le déplacement du personnage d'un point A vers un point B,
de la gauche vers la droite.

Le joueur peut avoir besoin de sauter ou s'accroupir pour éviter certains obstacles,
ou pour progresser dans le niveau (tirs ennemis, escaliers, environnement...).

Le joueur a la possibilité de revenir en arrière sur une très courte distance, au cas où il aurait
manqué de ramasser un objet, ou atteindre une surface particulière.

À la fin de chaque niveau, le joueur doit vaincre un "boss", qui se présente comme un ennemi plus
fort et plus résistant que les autres. La complexité et le gain de chaque boss augmentent au fil
des niveaux.

Des points de contrôle (checkpoints) sont présents à certains points stratégiques des niveaux.
Si le joueur meurt au cours du niveau, il reviendra au dernier point de contrôle atteint.
Le joueur a trois chances pour atteindre la fin du niveau. S'il meurt trois fois, les
points de contrôle atteints sont perdus, et il devra recommencer le niveau depuis le début.


## Caméra et vue

La caméra (le champ de vision) est fixée au joueur, et le suit dans sa progression
(de la gauche vers la droite). Cependant, le joueur peut retourner en arrière sur
une distance très limitée.

Le champ de vision actuel définit la zone limite que le joueur ne peux pas quitter en
reculant. Une fois la limite atteinte (le bord gauche de la fenêtre), il n'a pas d'autre
choix que d'avancer pour continuer à jouer.


## Déplacements

- Droite (avancer)
Touche par défaut : →

- Saut
Touche par défaut : Espace

- Accroupi
Touche par défaut : ↓

- Gauche (reculer)
Touche par défaut : ←

- Double saut (?)
Touche par défaut : Espace (x2)
À définir.


## Santé des personnages

Chaque entité vivante (joueur et ennemis) possède une quantité de vie initialisée à 100%.
Un dégât subit entraine la diminution de cette quantité de vie.

À 0%, l'entité meurt. Un ennemi qui meurt disparait, et peut laisser un butin pour le joueur.
La mort d'un "boss" entraine l'accomplissement d'un niveau.


## Mode Arcade

En dehors de toute progression liée à la Campagne (avec les différents niveaux, époques,
boss, etc...), il existe également un mode de jeu dit "Arcade" qui ne présente pas de boss
de fin. Le principe de ce mode est de courir autant que possible en évitant les obstacles
et les monstres, en atteignant le plus haut score possible.

Ce mode présente quelques mécaniques qui diffèrent de celles décrites ci-dessus :
* Le joueur avance automatiquement, et ne peut pas s'arrêter.
* La vitesse du joueur augmente progressivement, jusqu'à une certaine limite.
* Le joueur ne peut pas retourner en arrière.
* Il n'y a pas de point de contrôle (checkpoint) au cours du niveau.
* La mort du joueur entraine la fin de la partie.


## Score et pièces

Le score du joueur est calculé en fonction des pièces ramassées et ennemis tués au
cours du niveau. Le temps est aussi compté et un calcul s'opère à la fin du niveau
afin de donner un bonus au joueur.

Les pièces constituent la monnaie globale du jeu. Le joueur doit terminer un niveau
pour collecter les pièces qu'il a ramassées.


## Objets bonus

Chaque niveau présente des objets bonus d'apparence unique mais qui remplissent
la même fonction : la nourriture, qui restaure des points de vie. (d'autres restent
à définir plus tard)


## Boutique

La boutique est accessible depuis le menu principal du jeu, et permet au joueur
de dépenser les pièces ramassées au cours des différents niveaux. Il peut y acheter
des armes à usage unique, qui seront utilisées lors de la partie suivante.


## Paramètres

Le joueur peut régler certains paramètres du jeu afin de profiter d'une expérience
de jeu optimale. Il peut ajuster le volume général du jeu, ou seulement des musiques,
ou seulement des effets sonores.

Le jeu sera disponible en deux langues : français et anglais.


# Niveau 1 - Préhistoire

Objets :
	Pièces : Sillex
	Nourriture : Gigot de viande
	Arme 1 : Massue (dégâts)
	Arme 2 : Lance (portée)

Obstacles :
	Pierre
	Tronc d’arbre

Ennemis :
	Gardes de Sigma
	Phacochère

Boss :
	Apparence : Gros, habillé avec une peau de bête, barbu, monosourcil
	Arme : Gros os
	Attaque : Frappe simple
	Compétence spéciale : Charge


# Niveau 2 - Antiquité

Objet :
	Pièces : Pièce gravée
	Nourriture : Potions
	Arme 1 : Glaive (dégâts)
	Arme 2 : Arc (portée)

Obstacles :
	Ruines
	Buissons
	Relief du lieu

Ennemis :
	Gardes de Sigma
	Chiens errants

Boss :
	Apparence : Gladiateur, musclé 
	Arme : Trident
	Attaque : Frappe simple
	Compétence spéciale : Bouclier (se met dans une pose spéciale et se régénère quand on l’attaque)


# Niveau 3 - Moyen-Âge

Objets :
	Pièces : Écus
	Nourriture : Élixir
	Arme 1 : Épée (rapidité)
	Arme 2 : Hallebarde (portée)

Obstacles :
	Buissons
	Trous d'eau
	Ruines de châteaux forts

Ennemis :
	Gardes de Sigma
	Loups
	Bandits

Boss :
	Apparence : Chevalier
	Arme : Lance (Celle utilisé dans les tournois)(Très grande portée)
	Compétence spéciale : Charge avec son cheval et sa lance en avant. (Envoi en l'air le personnage)
	Attaque basique : Coup de lance en avant


# Niveau 4 - Renaissance

Objets :
	Pièces : Denier
	Nourriture : Antidotes
	Arme 1 : Fleuret (rapidité)
	Arme 2 : Tromblon (portée)

Obstacles :
	Charrettes
	Stands de marchés
	Trou de caniveau

Ennemis :
	Gardes de Sigma
	Soldats
	Voleurs

Boss :
	Apparence : Mousquetaire
	Arme : Flambert + Mousquet
	Attaque : Coup de flambert vertical
	Compétence spéciale : Tire avec son mousquet


# Niveau 5 - XXe siècle

Objets :
	Pièces : Monnaie
	Nourriture : Pansement
	Arme 1 : Pistolet (rapidité)
	Arme 2 : Grenade (dégâts)

Obstacle :
	Voiture
	Locomotive
	Fusée NASA

Ennemis :
	Gardes de Sigma
	Soldats
	Canons

Boss :
	Apparence : Tanque
	Arme : Canon
	Attaque : Tir de missile
	Compétence spéciale : Fonce sur le personnage en tirant en même temps


# Niveau 6 - XXIe siècle

Objets :
	Pièces : Billets
	Nourriture : Big Mac
	Arme 1 : Pistolet (dégâts)
	Arme 2 : Mitraillette (rapidité)

Obstacles :
	Poubelles
	Bouche d'incendie

Ennemis :
	Gardes de Sigma
	Policiers
	Drones

Boss :
	Apparence : Robot (style mini Metal Gear)
	Arme : Mitraillette + Lance-flammes
	Attaque : Tir de mitraillette horizontal, lance-flammes en diagonal
	Compétence spéciale : Tir aérien de missiles
	Remarque : Plus il perd de la vie plus le rythme de ses attaques accélère


# Niveau 7 - Futur Proche

Objets :
	Pièces : Puce électronique
	Nourriture : Pilule
	Arme 1 : Pistolet laser
	Arme 2 : Canon laser

Obstacles :
	Cargaison
	Vaisseau écrasé

Ennemis :
	Gardes de Sigma
	Sentinelle

Boss :
	Apparence : Oracle (style 343 Guilty Sparks)
	Arme : Laser
	Attaque : Tir laser
	Compétence spéciale : Impulsion électromagnétique


# Niveau final - Combat contre Sigma

Une fois que tous les niveaux ont été complétés, le joueur rencontre
le boss final : Sigma. Ils voyagent alors dans le temps pour mener
différents combats. À chaque fois que Sigma est "vaincu", il revit
en se téléportant à une autre époque. Le joueur revoit alors 4 niveaux
déjà complétés (seul le décor change), et Sigma voit ses capacités évoluer.

1ère étape (Préhistoire) :
	Teleport
	Pistolet Laser
	Enchaînement corps-à-corps

2ème étape (Moyen-Âge) :
	Teleport
	Canon laser
	Sabre laser

3ème étape (XXe siècle) :
	Gardes de Sigma apparaîssent

4ème étape (Futur Proche) :
	Teleport
	Pistolet Laser
	Sabre laser
	Canon laser
	Enchaînement corps-à-corps