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
L'utilisateur dispose d'un trombinoscope sur lequel il lui suffit de chercher la photo de la personne absente, ou de chercher le nom dans la barre de recherche dédiée.

![trombinoscope](/trombinoscope.png)
*Interface de l'application*

{{< encadres type="danger" titre="À noter" >}}
 Afin de respecter le droit à l'image du personnel de l'établissement, les photos et les noms présentés ici ont été générés par ordinateur, et ne sont en aucun cas des vrais personnes.
{{< /encadres >}}




Puis, par un simple clic 🖱️sur la photo de la personne concernée, elle est notée absente. *La photo devient alors rouge*. 

![Illustration rouge](/Capture-2.png)

Ainsi, il est très facile de voir si une personne du personnel a déjà été préalablement marquée absente par quelqu'un d'autre. 

{{<line_break>}}

Puis, ***un mail est envoyé*** à une liste de personnes prédéfinies (celles qui doivent savoir que la personne est absente)
![Exemple mail envoyé](/Absence-Email.png)
*Exemple de mail envoyé par le programme*

{{<line_break>}}

### Un programme complètement autonome

L'avantage pour l'utilisateur, c'est que j'ai créé une interface graphique pour éditer la base de données. Ainsi, l'utilisateur même sans connaissance en programmation peut mettre facilement à jour la base de données grâce à une interface dédiée.


![Illustration modify](/modify-absence.png)

Les quelques champs facilitent l'utilisation du programme.

{{< encadres type="" titre="Information complémentaire" >}}
  Il est aussi possible d'ajouter et de supprimer des personnes dans la base de donnée seulement par quelques clics.
  
{{< /encadres >}}

![Illustration modify](/Ajout-absence.png)

{{< encadres type="note" titre="💡Informations" >}}
  Statut : Terminé <br>
  Langage utilisé : <a href="https://www.php.net/">PHP </a> <br>
{{< /encadres >}}



