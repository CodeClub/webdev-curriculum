---
title: Stickers!
description: Cr�ez des stickers de robot amusants pour d�corer vos pages Web.  
layout: project
notes: "Stickers - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez cr�er tout un tas de stickers amusants que vous pouvez utiliser pour d�corer vos pages Web. Vous allez apprendre � utiliser des d�grad�s que changent graduellement d'une couleur � une autre pour que vos stickers aient l'air cool. 

![screenshot](images/stickers-finished.png)

# �tape 1�: Sticker codage color� {.activity}

Un d�grad� est un changement graduel d'une couleur � une autre. Les d�grad�s peuvent �tre utilis�s pour cr�er des effets cool. Vous allez les employer pour cr�er des stickers que vous pouvez utiliser sur vos pages Web. 

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-stickers" target="_blank">jumpto.cc/web-stickers</a>. 

	Le projet doit ressembler � �a�:

	![screenshot](images/stickers-starter.png)

+ Faisons un sticker 'I <3 Coding'. 

	Utilisez une `<div>` avec une classe `sticker` et un id `coding` pour que vous puissiez y appliquer un style�: 

	![screenshot](images/stickers-coding-error.png)


+ Hmm vous venez d'avoir une erreur�? C'est parce que '<' est un caract�re sp�cial en HTML. � la place de '<', vous devez utiliser le code sp�cial `&lt;`. 

	Mettez � jour votre code pour utiliser `&lt;` afin que l'erreur disparaisse. 

	![screenshot](images/stickers-coding-fixed.png)

	`<br>` donne une nouvelle ligne. 

+ Maintenant, rendons le sticker plus int�ressant. 

	Passez au fichier `style.css`. Vous allez voir que la classe `.sticker` vous a �t� fournie. Elle agencera les stickers sur la page et centrera leur contenu. 

	Souvenez-vous que vous avez ajout� l'id `coding` � votre sticker. Au bas de `style.css`, ajoutez le code suivant pour styliser le texte�:

	![screenshot](images/stickers-coding-font.png)

+ Maintenant, vous pouvez ajouter un d�grad� � l'arri�re-plan du sticker. Un d�grad� lin�aire passe d'une couleur � une autre le long d'une ligne droite.

	Ce d�grad� sera rouge au sommet et magenta en bas. Ajoutez le code d�grad� � votre style `coding` :

	![screenshot](images/stickers-coding-gradient.png)

+ Vous pouvez am�liorer le r�sultat en ajoutant un remplissage et des angles arrondis. 

	Ajoutez le code en surbrillance�:

	![screenshot](images/stickers-coding-padding.png)

	Le style `padding` ajoute un remplissage de 50 px au sommet et au bas et de 30 px � gauche et � droite. 


## Enregistrez votre projet {.save}

# �tape 2�: Sticker HTML & CSS {.activity}

Les d�grad�s peuvent aussi changer la couleur du centre vers les bords, c'est ce qu'on appelle un d�grad� radial. 

+ Cr�ons un sticker avec le texte `HTML & CSS.`  `&` est un autre caract�re qui n�cessite un encodage en HTML, le code est `&amp;`.

	Ajoutez le code en surbrillance pour cr�er un nouveau sticker�: 

	![screenshot](images/stickers-web-html.png)

+ Maintenant, passez � votre fichier `style.css` et ajoutez un style pour votre nouveau sticker.

	![screenshot](images/stickers-web-font.png)

	Le code `text-shadow` ajoute une ombre qui s'�tend de 2 px au-dessous et sur la droite du texte pour le faire ressortir. 

+ Maintenant passons au d�grad�. Cette fois, utilisons un d�grad� radial. La couleur variera du jaune au centre au orange puis au rouge. 

	![screenshot](images/stickers-web-gradient.png)

	Remarquez que les d�grad�s peuvent inclure de multiples couleurs, et pas seulement deux. 

+ Le sticker aura une bien meilleure apparence avec un peu de remplissage et une bordure arrondie. 

	Ajoutez le code en surbrillance�:

	![screenshot](images/stickers-web-padding.png)


## Enregistrez votre projet {.save}

##Challenge: Cr�ez votre propre sticker d�grad� {.challenge}

Maintenant, cr�ez votre propre sticker d�grad�. Essayez des d�grad�s lin�aires et radiaux en utilisant de multiples couleurs HTML. 

Il vous faudra�:

+ Ajouter une `<div>` avec le texte de votre sticker � `index.html` et lui donner la classe `sticker` ainsi qu'un nouvel `id`.
+ Ajouter un style pour l'`id` que vous avez choisi dans `style.css`. Vous pouvez copier l'un des styles de sticker que vous avez d�j� r�alis� et le modifier. 

Voici une liste de tous les noms de couleurs que vous pouvez utiliser�: [jumpto.cc/web-colours](http://jumpto.cc/web-colours), qui inclut les noms de couleurs comme `tomato`, `firebrick` et `peachpuff`.

Si vous voulez changer la couleur du texte, vous pouvez utiliser `color:`.

Voici un exemple de ce que vous pouvez faire avec de multiples couleurs dans un d�grad� lin�aire�:

![screenshot](images/stickers-save-robots.png)

## Enregistrez votre projet {.save}

# �tape 3�: Sticker robot fantaisiste {.activity}

Vous pouvez faire un sticker d�grad� en utilisant une image. Si vous utilisez une image avec un arri�re-plan transparent, alors le d�grad� se verra � travers. 

Vous pouvez aussi cr�er des d�grad�s dans plusieurs directions diff�rentes. 

+ Ajoutez un sticker � `index.html` en utilisant l'image `firerobot.png` :

	![screenshot](images/stickers-fire-html.png)

	Vous pouvez ajuster la `height` pour redimensionner l'image, la largeur changera automatiquement. 

+ Normalement, un d�grad� lin�aire part du haut vers le bas, mais vous pouvez utiliser `to` pour changer la direction. Par exemple�: `to top`, `to left`, ou `to right`.

	Pour un d�grad� diagonal, vous avez deux directions. Cet exemple utilise `to bottom left`.

	Ajoutez ce style � `style.css` pour donner � votre nouveaux stick robot un d�grad� diagonal et une bordure fantaisiste�:

	![screenshot](images/stickers-fire-gradient.png)

	Notez que vous pouvez utiliser `outline` pour cr�er une autre bordure en dehors de l'habituelle. 
	`outline-offset` donne l'�cart entre la bordure et le contour. 

+ Ajoutons un peu de texte � ce sticker. 

	Ajoutez un `<span>` contenant le texte "ROBOTS" � `index.html` et donnez-lui un id. 

	![screenshot](images/stickers-fire-span.png)

+ Le texte aura une meilleure apparence si vous le grossissez et le positionnez. 

	Pour positionner le texte, il vous faudra ajouter `position: relative;` � `#greensticker` et `position: absolute` � `#greentext`. Le positionnement est abord� plus en d�tails dans le projet `Construire un robot`. 

	Ajoutez le code suivant � `style.css`:

	![screenshot](images/stickers-fire-text-style.png)

+ Et pour le twist final, faisons pivoter le texte en utilisant `transform: rotate`.

	![screenshot](images/stickers-fire-rotate.png)

	Essayez de changer le nombre de degr�s de rotation du texte. 


## Enregistrez votre projet {.save}

##Challenge: Faire plus de stickers {.challenge}

Maintenant, essayez de faire plus de stickers en utilisant diff�rentes directions de d�grad�s et en ajoutant des images, du texte et en utilisant des bordures et des contours. 

Astuce�: Vous allez devoir ajouter du HTML et CSS pour chaque sticker. 

Vous pouvez copier et modifier l'un de vos exemples et faire des changements pour cr�er un nouveau sticker. 

Votre projet inclut d�j� un ensemble d'images de robot. Cliquez sur l'ic�ne images pour voir les images disponibles. 

![screenshot](images/stickers-images.png)

Cet exemple utilise un d�grad� lin�aire avec `to right`�:

![screenshot](images/stickers-green-html.png)

![screenshot](images/stickers-green-style.png)

## Enregistrez votre projet {.save}
