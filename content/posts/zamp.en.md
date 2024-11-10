---
title: "ZAMP"
description: "ZAMP is a simplified application for setting up a local development server with Apache, MySQL, and PHP without requiring technical configuration."
date: 2024-11-10T13:24:50+02:00
draft: false

author: ["Axel Thauvin"]

cover:
    image: "fishy.svg"
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


# ZAMP ? What is it ?:

ZAMP is designed to simplify the process of setting up a local development environment. Whether you're a seasoned developer or just starting out, ZAMP provides a hassle-free way to get your web server up and running with minimal effort. By integrating essential tools like Apache, MySQL, and PHP into a single package, ZAMP ensures that you can focus on coding rather than configuration.



{{< encadres type="warning" titre="⚠️ To take in consideration" >}}
 The app is still in development, and is intended to be open source, so the community can improve and customize it.
{{< /encadres >}}


## Overview

**ZAMP** is an all-in-one development stack for web developers, **providing everything you need** for ***local*** web development. It seamlessly integrates Apache, MySQL, and PHP, eliminating the need for individual installations.
With **zero configuration required**, ZAMP streamlines your development process, allowing you to focus solely on building your application. Additionally, starting all services is as simple as a single click, enhancing your productivity and efficiency.



![Zamp with projects loaded](./src/explanations/ZAMP-interface.png)

## Features

- **Zero Configuration**: Just install and run. No need to spend hours configuring your environment.
- **Integrated Management**: Easily manage Apache, MySQL, and PHP services from a single interface.
- **Extension Management**: Enable or disable PHP extensions with a simple checkbox interface.
- **Version Control**: Download and switch between different PHP versions with ease.
- **MySQL / MariaDB Launcher**: Simply click to open and close your SQL instance.
- **Drag and Drop Project Setup**: Simply drag and drop your project folders into ZAMP to get started.

## Installation

Currently, ZAMP is only available for Windows. We are actively working on making ZAMP available for macOS and Linux in the near future. Stay tuned for updates!

### Windows

1. Download the latest [ZAMP for Windows](https://github.com/Axthauvin/ZAMP/releases/download/Windows-0.0.2/zamp.Setup.0.1.2.exe).
2. Extract the archive to your preferred location.
3. Run `zamp.Setup.1.0.0.exe`.


## Usage

Once installed, you can access the following services:

- **Apache**: Clicking the start button 
![Start button](./src/explanations/Startbutton.png)

- **PHPMyAdmin**: PHP will automatically configure itself within the app. 
You can still change the version or the extensions using the dedicated areas.
![PHP config](./src/explanations/PHPConfig.png)

- **My SQL / Maria DB** : ZAMP uses MariaDB to run the SQL as it has binaries. MariaDB is retro compatible with MySQL, so you can still use workbench to access your server.

You can access the SQL server in the dedicated area

![SQL buttons](./src/explanations/MYSQL.png)

![Boutons SQL](/MYSQL.png)

{{< encadres type="note" titre="💡Informations" >}}
  Statut : En développement <br>
  Langage utilisé : <a href="https://www.electronjs.org/">Electron</a>, <a href="https://developer.mozilla.org/fr/docs/Web/HTML">HTML</a>, <a href="https://developer.mozilla.org/fr/docs/Web/CSS">CSS</a>, <a href="https://httpd.apache.org">Apache</a>
{{< /encadres >}}



