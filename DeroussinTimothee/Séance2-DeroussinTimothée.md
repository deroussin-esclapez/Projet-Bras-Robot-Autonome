# Rapport de séance – Projet bras robotique autonome

| | |
|---|---|
| **Date** | [date de la séance] |
| **Durée** | 4 heures |

## Objectif de la séance

L'objectif de cette séance était de modéliser les deux pièces qui constituent la base du robot :

- le **plateau tournant**, sur lequel repose le bras et qui tourne autour de l'axe vertical grâce au roulement Lazy Susan ;
- le **bâti**, partie fixe de la base, qui supporte le plateau tournant et accueille les composants électroniques.


## Partie 1 : modélisation du plateau tournant

Le plateau tournant est un disque qui fait le lien entre le roulement Lazy Susan et le bras.

Sur sa face inférieure, il comporte :

- un **logement circulaire** dans lequel vient se placer le roulement, avec quatre trous de fixation correspondant à ceux du roulement ;
- un **moyeu central** percé, destiné à recevoir l'entraînement de la rotation du plateau.

![Plateau tournant – face inférieure](plateau_dessous.png)

*Figure 1 : plateau tournant, face inférieure (logement du roulement et moyeu central)*

Sur sa face supérieure, il comporte deux **supports verticaux** percés, qui serviront à fixer le premier moteur du bras.

![Plateau tournant – face supérieure](plateau_dessus.png)

*Figure 2 : plateau tournant, face supérieure (supports de fixation du bras)*

Fusion n'était pas à jour sur mon ordinateur certaines cotes (notamment celles qui accueilleront les vis moteur) devront donc être vérifié avant d'être intégrée à l'assemblage.

## Partie 2 : première version du bâti

J'ai ensuite commencé la modélisation du bâti. La première version était une pièce unique de forme cylindrique, comportant une paroi extérieure et une couronne intérieure percée destinée à supporter le roulement et le plateau tournant.

![Première version du bâti](bati_v1.png)

*Figure 3 : première version du bâti, réalisée en une seule pièce*

Au cours de la modélisation, un problème est apparu : avec un bâti d'une seule pièce, l'intérieur est fermé et il devient **impossible d'accéder aux vis** pour fixer le plateau tournant sur le roulement lazy suzanne. Le montage du robot ne seraient donc pas réalisables.

Cette version a donc été abandonnée et le bâti a été repris à zéro.

## Partie 3 : nouvelle conception du bâti en plusieurs parties

Pour résoudre ce problème, le bâti est maintenant conçu en **plusieurs parties qui s'emboîtent**. Cette solution permet de fixer les composants sur chaque partie séparément, puis d'assembler le bâti une fois tout vissé.

J’ai commencé à modéliser la première partie : le bas du bâti. C’est un disque équipé d’ergots répartis sur deux cercles. Ces ergots servent à emboîter les parties supérieures du bâti, ce qui permet de les positionner et de les maintenir en place, tout en gardant un montage et un démontage simples.

![Bas du bâti](bati_bas.png)

*Figure 4 : bas du bâti, avec les plots d'emboîtement*

La modélisation des parties supérieures du bâti seront l'objet de la prochaines séance.

## Bilan et suite

Le plateau tournant est terminé mais nécessite une vérification. La première version du bâti a mis en évidence un problème d'accessibilité pour le montage, ce qui a conduit à une nouvelle conception en plusieurs parties emboîtables, dont le bas n'est pas encore totalement réalisé.

La prochaine étape sera de finir le bas du bati, de modéliser les parties supérieures du bâti, puis d'assembler le bâti avec le roulement et le plateau tournant afin de vérifier que l'ensemble s'ajuste correctement.
