---
title: "Application Absence"
date: 2022-03-24T21:18:50+02:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "Absence-app-icon.png"
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


# Fonctionnement du programme :

À la demande du chef  d'établissement du [Lycée Notre Dame de Bourg-la-Reine](http://www.indblr.asso.fr/), j'ai conçu et réalisé, en respectant  le cahier des charges demandé, un site internet permettant de signaler très vite à partir d'un smartphone ou d'un ordinateur, aux personnels concernés de l'établissement l'absence d'un de leurs collègues dès connaissance de l'information par un membre du conseil de direction.


# Description 
L'utilisateur dispose d'un trombinoscope sur lequel il lui suffit de chercher la photo de la personne absente.

![trombinoscope](https://github.com/Axthauvin/site-hugo/blob/main/static/trombinoscope.png?raw=true)

{{< encadres type="danger" titre="À noter" >}}
 Afin de respecter le droit à l'image du personnel de l'établissement, les photos et les noms présentés ici ont été générés par ordinateur
{{< /encadres >}}



Puis, par un simple clic 🖱️sur la photo de la personne concernée, elle est notée absente. *La photo devient alors rouge*. 

![Illustration rouge](https://github.com/Axthauvin/site-hugo/blob/main/static/Capture-2.png?raw=true)

Puis, un mail est envoyé à une liste de personnes prédéfinies (celles qui doivent savoir que la personne est absente)


### Un programme complètement autonome

L'avantage pour l'utilisateur, c'est que j'ai crée une interface graphique pour éditer la base de donnée. Ainsi, l'utilisateur même sans connaissance en programmation peut mettre facilement à jour la base de donnée grâce à une interface dédiée.


![Illustration modify](https://github.com/Axthauvin/site-hugo/blob/main/static/modify-absence.png?raw=true)

Les quelques champs facilitent l'utilisation du programme.

{{< encadres type="" titre="Information complémentaire" >}}
  Il est aussi possible d'ajouter et de supprimer des personnes dans la base de donnée seulement par quelques clics.
  
{{< /encadres >}}

![Illustration modify](https://github.com/Axthauvin/site-hugo/blob/main/static/Ajout-absence.png?raw=true)

{{< encadres type="note" titre="💡Informations" >}}
  Statut : Terminé <br>
  Langage utilisé : <a href="https://www.php.net/">PHP </a> <br>
{{< /encadres >}}

### Liens 

{{< button text="Voir sur github" path="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">}}

{{< chat cactus-comments >}}


