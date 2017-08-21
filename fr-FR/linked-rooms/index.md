---
title: Salons Li�s
description: Cr�er un projet Web avec plusieurs 'salons' li�s entre eux 
layout: project
notes: "Linked Rooms - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous allez cr�er un r�seau de salons li�s, dans lequel chaque salon est une page Web diff�rente que vous pouvez d�corer avec HTML. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/ba5d27ec68?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/rooms-hall-finished.png">
</div>

__Instructions__: Cliquez sur les portes pour vous d�placer entre les salons.

# �tape 1�: �tablir un lien avec une autre page Web du m�me projet {.activity}

Les projets Web peuvent �tre constitu�s d'un grand nombre de fichiers HTML li�s entre eux. 

## Liste de contr�le de l'activit� { .check}

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-rooms" target="_blank">jumpto.cc/web-rooms</a>. 

	Le projet doit ressembler � �a�:

	![screenshot](images/rooms-starter.png)

+ Le trinket devrait se lancer automatiquement et vous amener dans le Hall

	![screenshot](images/rooms-hall-start.png)

+ Observez la liste d'onglets de fichier pour ce trinket. Pouvez-vous voir `tvroom.html`�? Cliquez dessus.

	![screenshot](images/rooms-tvroom-html.png)

	Il s'agit d'un autre fichier html dans le m�me projet. 


+ Pour aller vers `tvroom.html` vous devez ajouter un lien dans `index.html`. 

	Ajoutez le code surlign� � l'int�rieur de la balise `<div>` avec la classe `room`: 

	![screenshot](images/rooms-link-tvroom.png)

+ Testez votre trinket en cliquant sur le lien __Salon TV__ pour voir la page Web `tvroom.html`.

	Notez que `tvroom.html` poss�de aussi son propre fichier de style `tvroom.css` qui d�finit l'agencement de cette page. 

	![screenshot](images/rooms-tvroom-unstyled.png)

	
##Challenge: Ajouter un autre lien {.challenge}

Ajouter un lien `<a>` sur la page Web `tvroom.html` pour revenir � la page Web Hall qui est appel�e `index.html`. Le texte du lien doit �tre 'Hall'.

La page Web Salon TV doit avoir un lien cliquable comme suit�:

![screenshot](images/rooms-hall-link.png)

Assurez-vous de tester votre code. Vous devriez pouvoir vous d�placer du Hall � Salon TV et revenir en cliquant sur les liens.  


## Enregistrez votre projet {.save}

# �tape 2�: Ajouter un autre salon {.activity}

Maintenant ajoutons un autre salon, un __Salon de jeux__. 

+ Cliquez sur le bouton ajouter une page __+__ :

	![screenshot](images/rooms-add-page.png)

	Inscrivez `gamesroom.html` comme nom de page�:

  	![screenshot](images/rooms-games-html.png)

+ Le HTML pour le __Salon de jeux__ est tr�s similaire � `tvroom.html` donc __copiez_ ceci et__collez-le__ dans `gamesroom.html`.
	
	Modifiez les objets mis en relief pour qu'ils indiquent Jeux et non TV�:

	![screenshot](images/rooms-games-html2.png)	

+ Votre `gamesroom.html` utilise maintenant `gamesroom.css` qui n'existe pas encore. 

	Cr�ez `gamesroom.css` en cliquant sur le bouton ajouter une page __+__. 


+ Le CSS pour le __Salon de jeux__ est tr�s similaire � `tvroom.css` donc __copiez_ ceci et__collez-le__ dans `gamesroom.css`.

	![screenshot](images/rooms-add-games-css.png)

+ Ajoutez un lien du Hall vers le Salon de jeux�:

	![screenshot](images/rooms-hall-games.png)

+ Testez votre projet en cliquant sur le lien du Salon de jeux

	Le __Salon de jeux__ doit ressembler � ceci�:

	![screenshot](images/rooms-games-before.png)

	Pas tr�s excitant, mais vous pouvez corriger cela dans le prochain challenge. 

## Enregistrez votre projet {.save}

##Challenge: Styliser et lier le Salon de jeux {.challenge}

Modifiez le HTML et le CSS pour le __Salon de jeux__ de mani�re � ce que la page Web ressemble � ceci�: 

![screenshot](images/rooms-games-challenge.png)

Indice�: Il vous faudra modifier la couleur de l'arri�re-plan, la couleur de la police et la couleur de la bordure dans `gamesroom.css`. La couleur vert clair est appel�e `chartreuse`.  

Indice�: Il vous faudra ajouter un lien `<a>` dans `gamesroom.html` qui dirigera vers `hall.html`.

## Enregistrez votre projet {.save}

# �tape 3�: Faire en sorte que les liens ressemblent � des portes {.activity}

Les liens ne doivent pas �tre simplement du texte. Faites une porte cliquable en utilisant une balise `<div>`.

## Liste de contr�le de l'activit� { .check}

+ Ouvrez `index.html` et ajoutez une balise `<div>` autour du lien textuel __Salon TV__. Cela doit �tre fait � l'int�rieur de la balise `<a>` pour qu'il soit cliquable.

  Ajoutez `id="hall2tv"` pour l'�tiqueter comme la porte depuis le Hall vers le Salon TV pour pouvoir appliquer un style � la porte. 

  ![screenshot](images/rooms-tvroom-div.png)  

+ Cliquez sur l'onglet `style.css`, allez au bas de la page et ajoutez le CSS suivant pour modifier la taille et la couleur de la porte�:

	![screenshot](images/rooms-door-css1.png)

+ Testez votre page Web en cliquant n'importe o� sur la porte, pas seulement sur le texte.

+ Maintenons, essayons d'am�liorer l'apparence de porte en ajoutant une bordure autour de trois c�t�s�:

	![screenshot](images/rooms-door-css2.png)

+ Puis ajoutons du CSS pour que le texte sur la porte ait un meilleur rendu�:

	![screenshot](images/rooms-door-css3.png)

+ Vous avez probablement remarqu� que la porte flotte dans les airs. Corrigeons cela en positionnant la porte � l'int�rieur du salon.

	![screenshot](images/rooms-door-position.png)	

+ Testez votre page Web en cliquant sur la porte pour aller dans le __Salon TV__.

## Enregistrez votre projet {.save}

##Challenge: Ajouter plus de portes�! {.challenge}

Transformez les autres liens de votre projet en portes de la m�me mani�re. 

Pour chaque porte�:

+ Modifiez le lien de la porte pour utiliser une balise `<div>` avec un id comme `hall2games` pour pouvoir y appliquer un style. 

	Par exemple�: 

	`<a href="gamesroom.html"><div id="hall2games">Games Room</div></a>`

+ Ajoutez du CSS pour l'id de la porte au fichier `.css` pour son salon. Utilisez _copier_ et _coller_ pour gagner du temps. Vous pouvez faire en sorte que chaque porte ait l'air diff�rente si vous le souhaitez. 

+ Positionnez la porte en utilisant `bottom:` et `left:` ou `right:`.

Le Hall peut ressembler � �a�:

![screenshot](images/rooms-hall-doors.png)

Le Salon TV devrait ressembler � quelque chose comme �a�:

![screenshot](images/rooms-tvroom-door.png)	


# �tape 4�: Ajouter une image d'arri�re-plan {.activity}

D�corons le hall avec une image d'arri�re-plan.

## Liste de contr�le de l'activit� { .check}


+  Modifiez le `style.css` pour ajouter une image d'arri�re-plan au Hall�:

	![screenshot](images/rooms-hall-decorated.png)	

	L'image sera r�p�t�e pour remplir tout le salon. 


## Enregistrez votre projet {.save}

##Challenge: Ajouter un fond d'�cran au Salon de jeux {.challenge}

Pouvez-vous d�corer le salon de jeux avec une image d'arri�re-plan�?

Vous pouvez utiliser l'image d'arri�re-plan `space-invader.png` qui est incluse dans votre projet. 

Pour ce faire�:

+ Ajoutez une `background-image:` au CSS `.room` pour le Salon de jeux. 

Le salon d�cor� devrait ressembler � �a�:

![screenshot](images/rooms-games-finished.png)	

## Enregistrez votre projet {.save}

##Challenge: Personnalisez-le�! {.challenge}

Ajoutez plus de salons � votre projet. Souvenez-vous que vous pouvez utiliser __copier__ et __coller__ pour �conomiser du temps, puis seulement modifier les choses qui doivent �tre diff�rentes. 

Pour chaque salon�:

+ Cr�ez un fichier `.html`
+ Ajoutez plus de liens vers et � partir du nouveau 'salon'.
+ Cr�ez un fichier `.css` avec les styles pour votre nouveau salon et ses portes

Vous pouvez modifier la `background-color:` pour chaque salon. Cliquez sur l'ic�ne images pour voir les images d'arri�re-plan que vous pouvez choisir�:

![screenshot](images/rooms-images.png)	

## Enregistrez votre projet {.save}

