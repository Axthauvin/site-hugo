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
    text : "Edit post"
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

[Pathfinding](https://en.wikipedia.org/wiki/Pathfinding) consists of finding a way to move in an environment between a starting point and an end point, taking into account different constraints

# Description 
The program consists of taking the player from one point to another using the shortest path.
The player is represented by the red square 🟥.


When the mouse is clicked🖱️, it will automatically move towards it avoiding the walls.

The interesting part was to add the notion of ***constraints***; which aims to add obstacles on a path (for example traffic jams), which slow down the character (represented by the blue squares 🟦).
Thus, the program must determine the fastest path, taking into account its length, as well as its constraints.



{{< encadres type="note" titre="💡Informations" >}}
  Status : Completed <br>
  Language used : <a href="https://www.python.org/">Python </a> <br>
  Modules : <a href="http://tkinter.fdex.eu/doc/intro.html">Tkinter</a> | <a href="https://pypi.org/project/pathfinding/">Pathfinding</a> <br>
{{< /encadres >}}

### Liens 

{{< button text="See on github" path="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">}}


