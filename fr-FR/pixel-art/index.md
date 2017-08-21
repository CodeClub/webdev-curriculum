---
title: Pixel Art
description: Cr�er un �diteur de pixel art. 
layout: project
notes: "Pixel Art - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez cr�er un �diteur de pixel art. En plus d'utiliser le HTML et le CSS, vous allez apprendre � utiliser le JavaScript pour ajouter de l'interactivit� � votre projet.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/0e102a306b?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/pixel-art-final.png">
</div>

__Comment utiliser l'�diteur__: Cliquez sur une couleur de la palette pour choisir la couleur de votre feutre puis cliquez sur les pixels pour changer leur couleur.

# �tape 1�: Cr�er une grille de pixels {.activity}

Cr�ons une grille de pixels que vous pouvez utiliser pour cr�er du pixel art. Le CSS fournit des styles de tableau pour les grilles et des agencements de tableau. 

Les tableaux contiennent des lignes qui contiennent des cellules. Vous allez cr�er un tableau avec un arri�re-plan noir, puis placer des pixels blancs � l'int�rieur. 

## Liste de contr�le de l'activit� { .check}

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-pixel" target="_blank">jumpto.cc/web-pixel</a>. 

	Le projet doit ressembler � �a�:

	![screenshot](images/pixel-starter.png)

+ Ajouter le html suivant dans le `<body>` de votre fichier `index.html` pour cr�er une `<div>` comme conteneur de votre pixel art et donnez-lui un id `art` pour pouvoir y appliquer un style�:

	![screenshot](images/pixel-art-art.png)

+ Maintenant, allez dans votre fichier `style.css` et ajoutez la stylisation de tableau pour l'art `<div>`.

	![screenshot](images/pixel-art-style.png)

	Cela cr�e un tableau avec une bordure et d�finit l'espacement � l'int�rieur de la grille. 

	Il n'a pas l'air tr�s int�ressant pour l'instant, vous devez placer des lignes de pixels � l'int�rieur. 

 + Maintenant, retournez � ton fichier `index.html` et ajoutez une ligne de 3 pixels � l'int�rieur de l'art `<div>`�:

	![screenshot](images/pixel-art-row.png)
	
	 Remarquez que les lignes de trois pixels sont les m�mes. Saisissez la premi�re, puis faites un copier/coller pour cr�er les autres. 

 	Cette fois vous utilisez des classes pour styliser les divisions car il y en aura beaucoup. 

 + Ajoutez le style suivant pour les lignes et les cellules�;

	![screenshot](images/pixel-art-row-style.png)

 	Maintenant, vos pixels s'aligneront dans une grille avec des lignes noires autour. 

 + Ajoutez maintenant deux autres lignes de pixels pour cr�er une grille 3 x 3. Souvenez-vous d'utiliser la fonction copier/coller pour gagner du temps. 

	![screenshot](images/pixel-art-grid-3.png)
	
    
##Challenge: Redimensionner votre grille {.challenge}

3 x 3 est une grille plut�t petite pour du pixel art. Pouvez-vous la rendre plus grande�? 8 x 8 est une bonne taille pour du pixel art. 

Essayez d'utiliser la fonction couper/coller plut�t que de tout saisir. 

![screenshot](images/pixel-art-grid-8.png)

## Enregistrez votre projet {.save}

# �tape 2�: Colorer les pixels {.activity}

Le HTML est utilis� pour organiser votre contenu et le CSS pour le styliser. Le JavaScript est un langage de programmation qui peut �tre utilis� pour modifier une page Web et la fa�on d'interagir avec. 

Vous pouvez utiliser le HTML et le CSS pour d�finir la couleur de l'arri�re-plan des pixels individuels, mais ce sera tr�s long�! Au lieu de �a, vous allez ajouter un peu de code en JavaScript pour colorer les pixels automatiquement lorsque vous cliquez dessus. 

+ En JavaScript, le code est plac� dans une `function` qui peut �tre appel�e quand nous souhaitons faire appel � ce code. 

	Vous allez cr�er une fonction appel�e `setPixelColour`

	La fonction `setPixelColour` doit savoir de quel pixel il faut modifier la couleur, c'est un `input`.

	Ajoutez le code suivant au fichier `script.js` pour d�finir la couleur d'arri�re-plan d'un pixel�:

	![screenshot](images/pixel-art-set-pixel-colour.png)

	Remarquez que `backgroundColor` utilise les d�nominations de couleur am�ricaines. 

+ Nous devons maintenant faire appel � cette fonction pour qu'elle intervienne lorsqu'on clique sur un pixel.

	Le HTML utilise `onclick` pour appeler une fonction lorsqu'un �l�ment est cliqu�. Vous allez devoir faire de 'this' l'entr�e pour que votre fonction sache de quel pixel il faut modifier la couleur. 

	Allez dans `index.html` et ajoutez le code suivant au premier pixel�:

	![screenshot](images/pixel-art-onclick.png)

+ Testez votre code en cliquant sur le premier pixel. Il devrait devenir noir�:

	![screenshot](images/pixel-art-black.png)

	Vous n'avez ajout� que le code `onclick` au premier pixel, donc �a ne fonctionnera pas encore pour les autres pixels. 


##Challenge: Rendre tous les pixels cliquable {.challenge}

Pouvez-vous rendre tous les pixels cliquables�? Utilisez la fonction couper/coller pour aller plus vite. 

Cr�ez un petit morceau de pixel art. 

![screenshot](images/pixel-art-black-example.png)

Astuce�: Vous pouvez cliquer sur __Autorun__ pour supprimer tous les pixels. 

# �tape 3�: Ajouter une palette de couleur {.activity}

Avez-vous trouv� ennuyeux de ne pas pouvoir modifier la couleur d'un pixel pour la rendre blanche � nouveau en cas d'erreur�? Corrigeons cela en cr�ant une palette de couleurs, pour que vous puissiez cliquer sur une couleur et changer le feutre. 

+ D'abord, cr�ez un style de feutre. 

	Ajoutez le code suivant au bas de votre fichier `style.css`�:

	![screenshot](images/pixel-art-pen.png)

+ Maintenant, cr�ez des couleurs de feutre noire et blanche qui utilisent ce style. 

	Ajoutez le code suivant � votre fichier `index.html` apr�s le `<body>`�:

	![screenshot](images/pixel-art-palette.png)

	`style=` vous permet d'ajouter du CSS � l'int�rieur de votre HTML, ce qui est pratique ici. 

+ Vous voulez pouvoir modifier la couleur du feutre lorsqu'une couleur de la palette est cliqu�e. 

	Des variables sont utilis�es pour stocker les informations. Cr�ons une variable penColour dans `script.js`.

	Ajoutez le code suivant au sommet du fichier�:

	![screenshot](images/pixel-art-pencolour.png)

	Puis ajoutez une fonction pour modifier la penColour�:

	![screenshot](images/pixel-art-set-pen.png)

+ Il vous faudra aussi utiliser la couleur du feutre lorsque vous modifiez la couleur d'un pixel. 

	Modifiez la fonction `setPixelColour` pour utiliser la variable `penColour` au lieu de `black`�:

	 ![screenshot](images/pixel-art-use-pen.png)

+ Vous devez maintenant faire appel � la fonction `setPenColour` lorsqu'un feutre de couleur est cliqu�. 

	Ajoutez le code `onclick` en surbrillance � vos couleurs de feutre�:

	![screenshot](images/pixel-art-palette-onclick.png)

+ Maintenant, voyez si vous pouvez faire basculer la couleur du feutre du noir au blanc pour remplir ou supprimer des pixels.


## Enregistrez votre projet {.save}

##Challenge: Ajouter plus de couleurs � la palette {.challenge}

Pouvez-vous ajouter plus de couleurs � la palette�? Choisissez les couleurs avec lesquelles vous voulez cr�er un pixel art. 

Puis cr�ez quelques pixels art.

Indice�: La couleur vert clair est appel�e `chartreuse`.

![screenshot](images/pixel-art-final.png)

Demandez au leader de votre club si vous pouvez utiliser l'outil de capture d'�cran de Windows ou une alternative pour enregistrer une copie de votre pixel art sous forme d'image. 

## Enregistrez votre projet {.save}

