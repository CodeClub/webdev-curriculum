---
title: Aurores — Notes pour les leaders du club
---

#Introduction:
Dans ce projet, les enfants apprendront � animer une sc�ne simple en utilisant CSS. Ils utiliseront la r�gle @keyframes en CSS pour animer diff�rentes propri�t�s d'images et de divisions.

#Ressources en ligne

Nous recommandons d'utiliser [trinket](https://trinket.io/) pour �crire du HTML & CSS en ligne. Ce projet contient les trinkets suivants�:

+ [Point de d�part 'Sunrise'](https://trinket.io/html/web-sunrise)

Des enfants peuvent aussi utiliser ce trinket vide [(jumpto.cc/html-blank)](http://jumpto.cc/html-blank) pour �crire leur propre code HTML & CSS, ou ils peuvent utiliser ce trinket mod�le [(jumpto.cc/html-template)](http://jumpto.cc/html-template).

Il y a aussi un trinket contenant une solution d'exemple � tous les challenges�:

+ ['Sunrise' termin�](https://trinket.io/html/abcc0284a3)

#Ressources hors ligne
Ce projet peut �tre [termin� hors ligne](../offline.html) si d�sir�. Vous pouvez acc�der aux ressources du projet en cliquant sur le lien 'T�l�charger mat�riaux du projet' pour ce projet. Ce lien contient un dossier 'Ressources du projet', laquelle inclut des ressources dont les enfants auront besoin pour terminer ce projet en mode hors ligne. Assurez-vous que chaque enfant ait acc�s � une copie de ces ressources. Ce dossier inclut les fichiers suivants�:

+ template/index.html
+ template/prefix.js
+ template/style.css
+ sunrise/index.html
+ sunrise/style.css
+ sunrise/prefixfree.js
+ sunrise/boat.png
+ sunrise/cloud.png
+ sunrise/helicopter.png
+ sunrise/rainbow.png
+ sunrise/sun.png

Vous pouvez aussi trouver une version termin�e des challenges de ce projet dans la section 'Ressources b�n�voles', qui contient�:

+ sunrise-finished/index.html
+ sunrise-finished/style.css
+ sunrise-finished/prefixfree.js
+ sunrise-finished/boat.png
+ sunrise-finished/sun.png
+ sunrise-finished/rainbow.png

#Objectifs d'apprentissage
+ Stylisation et animation avec CSS�:
	+ Introduction de la r�gle `@keyframes` pour d�finir des �tapes dans une animation.
	+ Renforcement de l'utilisation des propri�t�s pour d�finir la taille, la forme, la position et la coupe des �l�ments d'une page Web.

Ce projet couvre des �l�ments des composantes suivantes de [Raspberry Pi Digital Making Curriculum](http://rpf.io/curriculum):

+ [Conception de ressources 2D et 3D](https://www.raspberrypi.org/curriculum/design/creator).

#Challenges
+ "Animation diagonale" - modification de l'animation des propri�t�s `@keyframe` � utiliser � gauche�:;
+ "Am�liorer le ciel" - ajouter plus d'images cl�s et param�trage de l'arri�re-plan:.
+ "Plus d'animations" - animer plus d'images ou d'�l�ments en utilisant diff�rentes propri�t�s CSS. 

#Questions fr�quemment pos�es

+ Ce projet utilise la biblioth�que javascript `prefixfree.js` pour permettre une compatibilit� des animations entre les navigateurs. Si cette biblioth�que n'est pas utilis�e, alors les enfants utilisant des anciens navigateurs devront d�clarer une animation pour leur navigateur, par exemple�:

```
animation: sky 10s infinite; 		  	// pour tous les navigateurs plus r�cents
-webkit-animation: sky 10s infinite;  	// pour les navigateurs Webkit (Chrome, Safari...)
-moz-animation: sky 10s infinite;     	// pour les navigateurs Mozilla
-o-animation: sky 10s infinite;       	// pour les navigateurs Opera
-ms-animation: sky 10s infinite;		// pour les navigateurs Microsoft 
```
