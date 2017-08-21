---
title: Lever de Soleil
description: Cr�er un lever de soleil anim� 
layout: project
notes: Lever de soleil - mat�riaux
...

# Introduction { .intro}

Dans ce projet, vous apprendrez � utiliser le CSS pour cr�er un lever de soleil anim�.

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/abcc0284a3?outputOnly=true&start=result" width="600" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="images/sunrise-final.png">
</div>

# �tape 1�: Cr�er le soleil { .activity}

Commen�ons en ajoutant une image pour le soleil et en le positionnant avec un peu de CSS.

## Liste de contr�le de l'activit� { .check}

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-sunrise" target="_blank">jumpto.cc/web-sunrise</a>. 

    Le projet doit ressembler � �a�:

	![screenshot](images/sunrise-starter.png)

+ Regardez � l'int�rieur du `body` de votre fichier `index.html` et vous trouverez les �l�ments de `div` pour le ciel et la mer.

    ```
    <div id="sky">
    </div>
    
    <div id="sea">
    </div>
    ```

+ Une image pour le soleil est d�j� incluse dans votre projet. 

    Ajoutez l'image � l'int�rieur de la `div` soleil en incluant un id pour pouvoir y appliquer un style�:

    ![screenshot](images/sunrise-sun-image.png)

+ Whoa, l'image est grande. Allez dans `style.css` et ajoutez le CSS pour r�gler la hauteur de l'image�:

    ![screenshot](images/sunrise-sun-height.png)

    Notez que la largeur est mise � jour automatiquement pour garder les m�mes proportions. 

+ Enfin, ajoutons un peu de code pour positionner le soleil�:

    ![screenshot](images/sunrise-sun-position.png)


## Enregistrez votre projet {.save}

# �tape 2�: Animer le lever de soleil { .activity}

Pour animer votre lever de soleil, vous devez d�finir comment le soleil bouge et combien il met de temps � se lever.

Pour ce faire, vous devez d�finir une liste __images cl�s__. Chaque image cl� d�finit les propri�t�s CSS d'un �l�ment � un point sp�cifique de l'animation. 

## Liste de contr�le de l'activit� { .check}

+ D'abord, vous devez utiliser `@keyframes` pour cr�er une nouvelle animation appel�e lever de soleil. 

    Ajoutez ce code CSS � la fin de votre fichier `style.css` :

    ```
    @keyframes sunrise {
        0% {top: 90%;}
        100% {top: 0;}
    }
    ```

    Ce code indique au soleil o� se positionner au d�but (`0%`) et � la fin (`100%`)de l'animation.

    Puisque le soleil est � l'int�rieur de la `div` ciel, les positions `top` et `left` que vous donnez sont comprises dans le ciel, avec `top�: 100%` �tant le bas du ciel, et non le bas de la page Web.


+ Maintenant que vous avez cr�� une animation `sunrise`, vous devez simplement dire � votre soleil de l'utiliser�! 

    Ajoutez le code en surbrillance au CSS de votre soleil�:

    ![screenshot](images/sunrise-sunrise.png)

    Il indique � votre soleil de passer 10 secondes � animer un lever de soleil.

+ Pour lancer l'animation � nouveau dans Trinket, cliquez simplement sur **Autorun**. 

## Enregistrez votre projet {.save}

##Challenge: Animation diagonale {.challenge}
Pouvez-vous ajouter du code � votre animation `sunrise` pour que votre soleil commence en bas � gauche du ciel et se d�place en diagonale par rapport � sa position pour se retrouver centr� au sommet�?

Vous pouvez utiliser la propri�t� `left` pour le faire, par exemple�:

```
left: 40%;
```

![screenshot](images/sunrise-left.png)

## Enregistrez votre projet {.save}


# �tape 3�: Animation infinie { .activity}

Faisons en sorte que l'animation se r�p�te � l'infini.

## Liste de contr�le de l'activit� { .check}

+ Si vous voulez que le soleil se l�ve puis se couche, ajoutez plus d'images cl�s � votre animation�:

    ```
    @keyframes sunrise {
        0%   {top:90%; left:0;}
        33%  {top:0; left:40%; }
        66%  {top:0; left:40%; }
        100% {top:90%; left:80%; }
    }
    ```

    Cela signifie que l'animation commence et se termine avec le soleil au bas du ciel, et qu'il reste au sommet de 33�% � 66�% de l'animation.

+ Maintenant, vous devez simplement ajouter le mot `infinite` � l'animation `#sun` pour qu'elle tourne en boucle � l'infini�:

    ![screenshot](images/sunrise-infinite.png)

+ Testez votre animation. Le soleil se l�ve-t-il et se couche-t-il en boucle�? 


## Enregistrez votre projet {.save}

# �tape 4�: Animer le ciel { .activity}

L'animation n'est pas que pour les mouvements. Animons le ciel pour qu'il soit sombre la nuit.

## Liste de contr�le de l'activit� { .check}

+ Ajoutez une animation appel�e  `sky` � votre CSS�:

    ```
    @keyframes sky {
        0% {background: black}
        100% {background: lightblue}
    }
    ```

    Remarquez que cette fois vous animez la couleur du ciel, et non pas une position.

+ Ajoutez du code � votre ciel pour lui dire d'utiliser votre nouvelle animation�:

    ```
    animation: sky 10s;
    ```

    ![screenshot](images/sunrise-sky.png)

+ Cliquez sur **Autorun** pour tester votre animation. 

## Enregistrez votre projet {.save}

##Challenge: Am�liorer le ciel {.challenge}

Pouvez-vous changer l'animation du ciel pour qu'il soit en phase avec le soleil, qu'il reste bleu durant la journ�e et qu'il devienne sombre lorsque le soleil se couche�? Faites en sorte qu'il s'agisse d'une boucle. 

![screenshot](images/sunrise-sky-challenge.png)

##Challenge: Plus d'animations {.challenge}

Pouvez-vous animer une autre image�? Vous pouvez animer la position, la couleur, la forme, la taille, l'opacit� (seethroughness) ou tout ce � quoi vous pouvez penser. Essayez �galement de changer la dur�e de vos animations. 

Pour chaque objet que vous souhaitez animer, il vous faudra�:

+ L'inclure dans votre HTML avec un id
+ Ajouter un style pour l'id
+ Cr�er une r�gle @keyframes
+ Utiliser `animation:` dans le style pour utiliser l'animation que vous avez d�finie avec @keyframes 

Cliquez sur l'ic�ne image pour voir les images qui sont incluses dans le projet�:

![screenshot](images/sunrise-images.png)

Vous pouvez aussi mettre en ligne vos propres images si vous le souhaitez. 

N'oubliez pas de placer les objets dans la mer ainsi que dans le ciel�:

![screenshot](images/sunrise-boat.png)

Dans l'exemple, l'arc-en-ciel utilise l'opacit� pour obtenir un effet d'att�nuation�:

```
@keyframes fade {
  0%   {opacity: 0;}
  50%  {opacity: 100;}
  66%  {opacity: 0;}
  100%   {opacity: 0;}
}
```

Le bateau utilise une position de d�part n�gative pour que vous ne puissiez pas le voir pendant une partie de l'animation�:

```
 @keyframes left-right {
  0%    {left:-50%;}
  100%  {left:200%;}
}
```

## Enregistrez votre projet {.save}
