---
title: Magazine
description: Cr�er un site Web magazine � plusieurs pages. 
layout: project
notes: "Magazine - notes.md"
...

# Introduction { .intro}

Dans ce projet, vous apprendrez � utiliser le HTML et CSS pour cr�er une site Web magazine � plusieurs pages avec un agencement � deux colonnes. Vous r�viserez �gament beaucoup de techniques HTML et CSS d'autres projets. 

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/a41e4e1c5c?outputOnly=true&start=result" width="600" height="500" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/magazine-final.png">
</div>


# �tape 1�: En-t�te et arri�re-plan

Les sites Web de style magazine ont souvent beaucoup de petits objets sur une page. Tout d'abord, vous allez cr�er un en-t�te et un arri�re-plan pour votre magazine. 

## Liste de contr�le de l'activit� { .check}

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-magazine" target="_blank">jumpto.cc/web-magazine</a>. 

	Le projet doit ressembler � �a�:

	![screenshot](images/magazine-starter.png)

+ Ajoutons un en-t�te. 

	Vous pouvez trouver un meilleur titre pour votre magazine. 

	![screenshot](images/magazine-heading.png)

+ Pouvez-vous appliquer un style � l'en-t�te�?

	Voici un exemple, mais vous pouvez choisir votre propre style�:

	![screenshot](images/magazine-heading-style.png)

+ Maintenant, cr�ons un arri�re-plan int�ressant en utilisant un d�grad� et en choisissant une police pour le magazine. 

	Voici quelques exemples de style pour vous rapeller comment cr�er un d�grad�: 

	![screenshot](images/magazine-background.png)

## Enregistrez votre projet {.save}

# �tape 2�: Cr�er des colonnes

Les sites Web utilisent souvent plusieurs colonnes. Cr�ons un agencement � deux colonnes pour votre magazine. 

## Liste de contr�le de l'activit� { .check}

+ D'abord, cr�ez deux colonnes `div`.

	Ajoutez le HTML surlign� � `index.html`�:

	![screenshot](images/magazine-columns.png)

+ Maintenant, stylisez les divisions de colonnes pour que l'une soit flottante vers la gauche et l'autre vers la droite. 

	![screenshot](images/magazine-columns-style.png)

	Chaque colonne est inf�rieure � 50�%, il y a donc de la marge pour un remplissage. 

	Vous devez ajouter quelque chose � une colonne pour voir l'effet. 

+ Ajoutons une image de chaton au sommet de la colonne 2. 

	![screenshot](images/magazine-kitten.png)

	Remarquez sur l'image de chaton est positionn�e sur � peu pr�s la moiti� de la page, dans la seconde colonne. 

	C'est un peu gros�!

+ Utilisons `max-width: ` pour que les images s'adaptent � leur conteneur. 

	Ajoutez le style suivant � `style.css`.

	![screenshot](images/magazine-img-width.png)

	Il s'appliquera � toutes les images que vous utilisez dans votre magazine, et pas seulement au chaton.

+ Maintenant, ajoutez une classe `photo` � l'image pour que vous puissiez y appliquer un style�:

	![screenshot](images/magazine-photo.png)

+ Puis stylisez l'image pour y ajouter une ombre et une torsion afin que l'image sorte de la page�:

	![screenshot](images/magazine-photo-style.png)

	Faites quelques changements � moins que vous n'aimiez le r�sultat. 


# �tape 3�: Styliser les objets du magazine

Appliquons-nous � rendre l'agencement un peu plus int�ressant. 

## Liste de contr�le de l'activit� { .check}

+ Ajoutez une balise `div` autour de votre image avec une `class` et ajoutez un en-t�te `h2`�:

	![screenshot](images/magazine-item.png)

+ Maintenant, stylisez l'objet et l'en-t�te. 

	Voici un exemple, mais vous pouvez faire quelque changements�:

	![screenshot](images/magazine-item-style.png)

## Enregistrez votre projet {.save}

##Challenge: Ajouter des objets � la colonne de gauche {.challenge}

Pouvez-vous ajouter une liste ordonn�e et un sticker de texte d�grad� � la colonne de gauche�? 

Voici un exemple�:

![screenshot](images/magazine-challenge1-example.png)

Voici le code pour l'exemple, mais vous pouvez le changer ou faire le v�tre.

HTML�:

![screenshot](images/magazine-challenge1.png)

CSS�:

![screenshot](images/magazine-challenge1-style.png)


## Enregistrez votre projet {.save}


# �tape 4�: Ajouter une seconde page

Ajoutons une seconde page � votre site Web magazine. 

## Liste de contr�le de l'activit� {.check}

+ Ajoutez une nouvelle page � votre projet et nommez-la `page2.html`�:

![screenshot](images/magazine-page2.png)

+ La Page 2 sera tr�s similaire � la premi�re page de votre magazine pour que vous puissiez copier le html de `index.html` et le coller dans `page2.html`.

![screenshot](images/magazine-page2-html.png)

Remarquez que les deux pages utilisent le m�me `style.css`. Elles partageront donc le m�me style. 

+ Modifiez le titre `<h1>` par page2�: 

![screenshot](images/magazine-page2-h1.png)

+ Maintenant, il vous faudra des liens entre vos pages pour pouvoir acc�der � la page 2 et revenir � la premi�re page. 

Retourner � `index.html`. Ajoutez un lien dans une div � l'int�rieur de la colonne 2 dans `index.html`:

![screenshot](images/magazine-page2-link.png)

+ Testez qu'il est possible de cliquer sur votre nouveau lien et de passer � la page 2 de votre magazine. 

##Challenge: Ajouter un lien de retour � la premi�re page {.challenge}

Pouvez-vous ajouter un lien vers la `page2.html` pour pouvoir cliquer et revenir � la premi�re page�?

Indice�: Regardez le HTML que vous avez utilis� pour cr�er un lien vers la page 2. 

![screenshot](magazine-page1-link.png)

##Challenge: Remplir votre seconde page {.challenge}

Voici le code pour les exemples, mais vous pouvez modifier les `div` ou utiliser vos propres id�es.  

![screenshot](images/magazine-page2-challenge.png)

Cliquez sur l'ic�ne images pour voir les images qui sont disponibles � l'utilisation�:

![screenshot](images/magazine-images.png)

Souvenez-vous que vous pouvez mettre en ligne vos propres images pour les utiliser. Assurez-vous d'avoir les autorisations n�cessaires pour utiliser les images que vous mettez en ligne. 

![screenshot](images/magazine-upload-images.png)

# �tape 5�: Ajouter une animation

Ajoutons une animation amusante � votre magazine. 


## Liste de contr�le de l'activit� {.check}

+ Allez dans `index.html` et incluez l'image `greenrobot.png` au sommet de votre page. 

![screenshot](images/magazine-animation-image.png)

+ Maintenant, ajoutez le CSS pour animer votre robot�:

![screenshot](images/magazine-animation-css.png)


##Challenge: Ajouter une autre animation {.challenge}

Pouvez-vous ajouter une animation � la seconde page de votre magazine�? 

![screenshot](images/magazine-animation-challenge.png)


