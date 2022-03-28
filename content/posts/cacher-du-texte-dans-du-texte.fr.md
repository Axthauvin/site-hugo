---
title: "Cacher du texte dans du texte"
date: 2021-11-04T22:35:57Z
draft: false

description : Comment j'ai caché du texte dans du texte. En manipulant les bits du texte, j'ai réussi à cacher du texte dans du texte avec des caractères cachés.
author: ["Axel Thauvin"]

cover:
    image: "https://delante.co/wp-content/uploads/2019/11/hidden-text-definicja.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "Illustration"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
    responsiveImages: false
    

editPost:
    URL: "https://github.com/Axthauvin/site-hugo/blob/main/content"
    text : "Proposer des modifications"
    appendFilePath: true

params:
    ShowCodeCopyButtons: true
    ShowShareButtons: true
    ShowReadingTime: true
    linkFullImages: true
    ShowReadingTime: true



---

{{< encadres type="" titre="❔Où trouver le projet" >}}
  Le projet est actuellement hébergé sur <a href="https://cacherdutexte.github.io">https://cacherdutexte.github.io</a>
{{< /encadres >}}


### Comment j'ai caché du texte dans du texte
C'est une façon en manipulant les bits de cacher du texte dans du texte.
Imaginons la chaine de caractère :
```
Hacker
```
Que je veux cacher dans le message :
```
Bonjour, je suis Axel Thauvin
``` 

- Dans un premier temps, on vient récupérer la **représentation décimale dans la table UTF-8** de chaque caractère de la chaine `Hacker`.

  *Voici dans un tableau, la représentation décimale des 127 premiers caractères (aussi appelé tableau ASCII) :*
  ![Tableau ascii](https://github.com/Axthauvin/cacher-du-texte-dans-du-texte/blob/main/images/UTF8-TABLE.png?raw=true)


Pour l'exemple, nous allons prendre le caractère `H`.
Ici, sa représentation décimale est ***72*** (base 10).

- Ensuite nous allons convertir ce nombre en base 6 sur 4 'bits'
  # Pourquoi ?
  Si nous codons les lettres en base 6 sur 4 bits, nous aurons la représentation maximale de `5555` -> soit 6⁴ -> `1296` :
  *la valeur maximale que nous allons pouvoir exploiter dans ce tableau*
  
  En fait nous avons 5 **caractères invisibles** qui vont correspondrent aux chiffres de ces bits, que nous allons *cacher* dans notre texte.
  - *Pour le 0 il n'y a pas de caractère caché*
  - *Pour le 1 c'est le caractère unicode `\u200C`*
  - *Pour le 2 c'est le caractère unicode `\u200D`*
  - *Pour le 3 c'est le caractère unicode `\u200E`*
  - *Pour le 4 c'est le caractère unicode `\u200F`*
  - *Pour le 5 c'est le caractère unicode `\u034F`*
  
  # Exemple avec le `H`
  
  Ici la représentation décimale de `H` est ***72***.
  Sa représentation en *base 6 sur 4 bits* est `0200`.
  
  Je vais donc : 
  - Pas ajouter de caractère pour le 1er bit (car il vaut 0)
  - Ajouter le caractère `\u200D` pour le 2ème bit (car il vaut 2)
  - Pas ajouter de caractère pour le 3ème bit (car il vaut 0)
  - Pas ajouter de caractère pour le 4ème bit (car il vaut 0)
  
  ***Reprenons la chaine initiale***
  J'ai `Bonjour, je suis Axel Thauvin`.
  Je vais donc écrire : **Bo`\u200D`nj** juste pour le H
  
  ***Et je fais pareil avec tous les caractères de `Hacker`.***
  Ce qui me donne : 
  `Bo‍njou‍r‏,‌ j‍e‏ ‎su‍i͏s͏ A‍x‏e͏l ‎T‌hauvin` (généré avec mon programme, vous pouvez l'essayer sur mon site)
  
  ***Voilà le résultat :***
  ![Image gif](https://github.com/Axthauvin/cacher-du-texte-dans-du-texte/raw/main/images/VideoIllustration.gif)
  