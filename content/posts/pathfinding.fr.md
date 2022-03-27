---
title: "Pathfinding"
date: 2019-11-02T12:50:18+01:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "https://axthauvin.github.io/Projets/Python-Pathfinding/Pathfind-Game.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "Illustration"
    #caption: "Schéma illustrant le pathfinding"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
    responsiveImages: false

editPost:
    URL: "https://github.com/Axthauvin/site-hugo/blob/main/content"
    text : "Proposer des modifications"
    appendFilePath: true

ShowToc: true
TocOpen: true  

params:
    ShowCodeCopyButtons: true
    ShowShareButtons: true
    ShowReadingTime: true
    linkFullImages: true
    ShowReadingTime: true
    
---

# Introduction

Le [Pathfinding](https://fr.wikipedia.org/wiki/Recherche_de_chemin) consiste à trouver comment se déplacer dans un environnement entre un point de départ et un point d'arrivée en prenant en compte différentes contraintes

# Description 
Le programme consiste à emmener le joueur d'un point à un autre en utilisant le chemin le plus court.
Le joueur est représenté par le carré rouge 🟥.



Lors du clic de la souris🖱️, il se dirigera automatiquement vers celle ci en évitant les murs.

La partie interessante était d'ajouter la notion de ***contraintes***; qui a pour but d'ajouter des obstacles sur un chemin (par exemple des embouteillages), qui ralentissent le personnage (représentées par les carrés bleu 🟦).
Ainsi, le programme doit déterminer le chemin le plus rapide, en prennant en compte sa longueur, ainsi que ses contraintes.



{{< encadres type="note" titre="💡Informations" >}}
  Statut : Terminé <br>
  Langage utilisé : <a href="https://www.python.org/">Python </a> <br>
  Modules : <a href="http://tkinter.fdex.eu/doc/intro.html">Tkinter</a> | <a href="https://pypi.org/project/pathfinding/">Pathfinding</a> <br>
{{< /encadres >}}

### Liens 

{{< button text="Voir sur github" path="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">}}


