---
title: "Analyseur de parties Chess.com"
description: "Cette extension analyse vos parties directement sur Chess.com grâce à stockfish 17 lite, en affichant les meilleurs coups, des évaluations en temps réel et des superpositions visuelles minimalistes pour mieux comprendre chaque coup."
date: 2025-05-25T21:18:50+02:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "chess-analyser-icon.png"
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

<!-- <div align="center">
  <img src="img/icon.png" width="128" alt="Extension Icon" /> -->

Analysez vos parties directement sur [chess.com](https://www.chess.com/) !  
 Profitez de superpositions visuelles intelligentes, d’analyses instantanées des coups et améliorez votre jeu avec une interface simple et épurée.

{{< encadres type="warning" titre="⚠️ À noter" >}}
Ce projet est encore en cours de développement.
{{< /encadres >}}

---

![Gif de présentation](/presentation.gif)

## Installation

### Chrome (installation manuelle)

1. Clonez ou téléchargez ce dépôt.
2. Allez sur `chrome://extensions/`.
3. Activez le **mode développeur** (en haut à droite).
4. Cliquez sur **« Charger l’extension non empaquetée »** et sélectionnez le dossier de l’extension.

### Firefox (installation manuelle)

1. Allez sur `about:debugging#/runtime/this-firefox`.
2. Cliquez sur **« Charger un module complémentaire temporaire… »**.
3. Sélectionnez n’importe quel fichier du dossier de l’extension (ex. : `manifest.json`).
4. L’extension sera active temporairement jusqu’au redémarrage de Firefox.

> ✅ Une version Web Store et AMO sera bientôt disponible !

---

## Fonctionnalités

- Rendu intelligent de flèches comme sur Chess.com
- Analyse en temps réel des coups
- Intégration de l’évaluation (Stockfish lite 17)
- Léger et performant — fonctionne en toute discrétion en arrière-plan

---

## Captures & Démos

> Emplacement réservé pour les visuels à venir.

---

## 🤝 Contribuer

Les suggestions et pull requests sont les bienvenues !  
N’hésitez pas à ouvrir une issue ou proposer une fonctionnalité.

---

{{< encadres type="note" titre="💡Informations" >}}
Status : En cours <br>
Languages utilisés : <a href="https://developer.mozilla.org/fr/docs/Web/JavaScript">JS (#jsnatifesttellementbien) </a> <br>
{{< /encadres >}}
