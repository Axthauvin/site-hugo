---
title: "chess.com games analyser"
description: "This extension analyzes your games directly on Chess.com using Stockfish 17 Lite. It displays smart arrows, real-time evaluations, and minimal visual overlays to help you better understand each move."
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

Analyze your games directly on [chess.com](https://www.chess.com/)!  
 Get powerful visual overlays, instant move insights, and improve your game with a clean and minimal interface.

{{< encadres type="warning" titre="⚠️ To take in consideration" >}}
The extension is still in development.
{{< /encadres >}}

---

![presentation gif](/presentation.gif)

## Installation

### Chrome (manual install)

1. Clone or download this repo.
2. Go to `chrome://extensions/`.
3. Enable **Developer mode** (top right).
4. Click **“Load unpacked”** and select the extension folder.

### Firefox (manual install)

1. Go to `about:debugging#/runtime/this-firefox`.
2. Click **“Load Temporary Add-on…”**.
3. Select any file from the extension directory (e.g., `manifest.json`).
4. The extension will load temporarily until Firefox restarts.

> ✅ A Web Store & AMO version will be available soon!

---

## Features

- Smart arrow rendering like Chess.com
- Real-time move analysis overlay
- Evaluation integration (Stockfish lite 17)
- Minimal and performant — works silently in the background

---

## Screenshots & Demos

> Placeholder for future visuals.

## Contributing

Pull requests and suggestions are welcome!
Feel free to open issues or submit feature ideas.

<div align="center"> <img src="img/icon.png" width="64" /> 
<br/> <b>Happy analyzing!</b></div>

{{< encadres type="note" titre="💡Informations" >}}
Status : Over <br>
Languages used : <a href="https://www.php.net/">PHP </a> <br>
{{< /encadres >}}
