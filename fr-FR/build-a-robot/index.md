---
title: Construire un Robot
description: Apprenez � positionner des images pour fabriquer votre propre robot.
layout: project
notes: "Build a Robot - notes.md"
---

# Introduction { .intro}

Dans ce projet, vous apprendrez � positionner des images pour cr�er votre propre robot�!

![screenshot](images/robot-final.png)

# �tape 1�: Donner des yeux � votre robot { .activity}

Donnons des yeux � votre robot�!

## Liste de contr�le de l'activit� { .check}

+ Ouvrez ce trinket�: <a href="http://jumpto.cc/web-robot" target="_blank">jumpto.cc/web-robot</a>.

    Le projet doit ressembler � �a�:

	![screenshot](images/robot-starter.png)

+ Chaque image de ce projet poss�de son propre nom (ou __id__). Par exemple, le lien HTML pour les images des yeux et du visage (‘face’, ‘eyes1’ et ‘eyes2’ commen�ant � la ligne 8 de votre code) ressemblent � �a�:

```
<img id="face" ...>
<img id="eyes1" ...>
<img id="eyes2" ...>
```

+ Vous pouvez utiliser l'id d'une image pour lui donne son propre style, en utilisant le symbole `#`. Cela vous permet de styliser chaque image s�par�ment.

Cliquez sur le fichier `style.css`. Vous voyez comme la taille du visage du robot et celle des autres images sont diff�rentes�?

![screenshot](images/robot-id.png)

+ Ajoutez ce code CSS pour donner un style aux yeux du robot�:

```
#eyes1 {
    width: 200px;
}
```

Remarquez que vous stylisez uniquement l'image `eyes1`, en utilisant `#eyes1` dans votre CSS. Si vous pr�f�rez, vous pouvez utiliser `#eyes2` ou `#eyes3` � la place�!

![screenshot](images/robot-eyes-width.png)

+ Vous remarquez comme chaque image est affich�e l'une apr�s l'autre�? Il s'agit d'un positionnement __relatif__. Si vous voulez dire au navigateur exactement o� placer les yeux de votre robot, il vous faudra utiliser un positionnement __absolu__ � la place.

Ajoutez ces 3 lignes de code au CSS pour votre image `eyes1`�:

```
position: absolute;
top: 200px;
left: 100px;
```

Vous devriez voir les yeux de votre robot se d�placer au bon endroit sur votre robot.

![screenshot](images/robot-eyes-position.png)

Ce code CSS dit au navigateur � quelle distance afficher l'image du sommet/de la gauche de la page Web.

![screenshot](images/robot-eyes-position2.png)

Vous pouvez utiliser `bottom` au lieu de `top` pour dire au navigateur � quelle distance du bas de l'�cran afficher l'image, et utiliser `right` au lieu de `left`.

# �tape 2�: Donner une bouche � votre robot { .activity}

Donnons une bouche � votre robot�!

## Liste de contr�le de l'activit� { .check}

+ Ajoutez le code CSS suivant pour styliser votre image `mouth1`�:

```
#mouth1 {
    width: 50px;
    position: absolute;
    top: 200px;
    left: 200px;
}
```

+ La bouche de votre robot a l'air tr�s petite, et elle ne se trouve pas au bon endroit.

![screenshot](images/robot-mouth.png)

Pouvez-vous modifier cela en effectuant des changements dans votre CSS�?

## Enregistrez votre projet {.save}

##Challenge: Concevez votre propre robot {.challenge}
Utilisez ce que vous avez appris pour finir la conception de votre propre robot. Voici quelques exemples de ce � quoi votre robot pourrait ressembler�:

![screenshot](images/robot-examples.png)

## Enregistrez votre projet {.save}

##Challenge: Ajoutez vos propres images {.challenge}
Pouvez-vous trouver des images suppl�mentaires � ajouter � votre robot, et les positionner sur votre page Web�? Vous pouvez m�me remplacer le visage de votre robot par le v�tre�!

```
<img id="face" src="myFace.png">
```

## Enregistrez votre projet {.save} 
