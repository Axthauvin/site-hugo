---
title: "Word2pdf"
date: 2021-07-15T14:45:35+01:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "Word2pdf.png"
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


params:
    ShowCodeCopyButtons: true
    ShowShareButtons: true
    ShowReadingTime: true
    linkFullImages: true
    ShowReadingTime: true

---

# Introduction

Ce projet est une interface graphique du module [docx2pdf](https://pypi.org/project/docx2pdf/), qui consiste à convertir des fichiers docx en pdf.

# Description
### Un outil simple à trouver pour une utilisation efficace

Devoir chercher un site pour convertir ses words en PDF était trop pénible.
Aujourd'hui, je peux en quelques clics 🖱️ palier à ce problème.

![Illustration comment trouver Word2pdf](/Recherche-word2pdf.png)
Comme on peut le voir, il est très facilement accessible

### L'interface

![L'interface](/word2pdf-interface.png )
Je l'accorde, ce n'est pas l'interface la plus *sexy* au monde

{{< encadres-markdown type="note" titre="L'idée est simple, j'ai 2 options qui s'ouvrent à moi : " >}}
 - Convertir ***un fichier*** DOCX en PDF
 - Convertir ***tous les fichiers d'un dossier*** qui sont en DOCX en PDF
{{< /encadres-markdown >}}

![Process](/word2pdf-process.png )





