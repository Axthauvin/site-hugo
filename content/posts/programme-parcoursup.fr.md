---
title: "ParcoursupExplorer"
date: 2022-07-20T21:18:50+02:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "Parcoursup-app-icon.png"
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


{{< encadres type="danger" titre="⚠️ Cette page est encore en construction" >}}
 Afin de d'avoir la meilleur description du projet possible, je prends le temps de m'assurer que cette dernière soit travaillée au maximum avant de la publier.
{{< /encadres >}}


# Fonctionnement du programme :

Afin d'aider les lycéens dans leur orientation, j'ai réalisé un programme de statistiques, qui se basant sur les résultats des élèves des promotions ultérieures, de savoir quelles formations ont étées obtenues par les élèves en fonctions de leur spécialitées.
Le lycée qui souhaite disposer du programme doit alors remplir un fichier excel comportant la liste de toutes les formations où les élèves ont reçu au moins une proposition d'admission.

Une version de se site Internet a été vendue à l'Institut Notre Dame de Bourg la reine, et le site internet est disponible à cette adresse [ParcoursupExplorer pour l'Institut Notre Dame](https://programme-ind-sup.alwaysdata.net/)


![Page d'acceuil](/parcoursup-app%20main%20page.png)
*Interface de l'application*


# Description :

Le programme se découpe en 2 parties distinctes : 

- **Les propositions acceptées par les élèves** : Les formations où les élèves ont choisi d'aller au final

- **Les propositions faites aux élèves** : Le programme ressence alors toutes les formations où les élèves ont été acceptés en fonction de leur spécialités (example : Prépa MPSI ou une license non sélective en informatique)

## Propositions acceptées par les élèves

![Formation acceptées](/parcoursup-app%20accepted.png)
*Graphique montrant toutes les propositions acceptées par les élèves de la promotion 2023*

Ce graphique permet aux élèves de voir quels sont les choix principaux des élèves, et donc d'avoir une idée des catégories de formations.

Cette information est aussi utile pour le lycée, car cela lui donne une information quant aux informations les plus attractives pour les élèves.


## Propositions faites aux élèves

C'est cette partie qui est au centre du programme. Afin de mieux la comprendre, je vais décomposer l'interface.

![Page principale](/parcoursup-app%20propositions%20main.png)
*Page principale du programme*

Ainsi, l'élève doit sélectionner 2 spécialités, afin que le programme soit en mesure de ressortir toutes les formations qui ont été obtenues par les élèves avec les mêmes spécialités sur une année précédente.


![Choix spécialités](/parcoursup-app%20spes.png)
*Choix des spécialités*

Le programme trouve alors 64 alèves avec ces spécialités dans les années précédantes.

![Statistiques](/parcoursup-app%20all%20forma.png)
*Il est alors possible de sélectionner différents filtres tel que : le choix de l'option, rt le choix de la 3ème spécialité abandonnée.*



<!--



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

![Illustration modify](/Ajout-absence.png)  -->

{{< encadres type="note" titre="💡Informations" >}}
  Statut : Terminé <br>
  Langage utilisé : <a href="https://developer.mozilla.org/fr/docs/Web/JavaScript">Javascript</a>, <a href="https://php.net">PHP</a> | Library <a href="https://www.chartjs.org/">ChartJS</a> <br>
{{< /encadres >}}



