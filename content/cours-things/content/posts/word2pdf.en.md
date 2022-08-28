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
    text : "Edit post"
    appendFilePath: true


params:
    ShowCodeCopyButtons: true
    ShowShareButtons: true
    ShowReadingTime: true
    linkFullImages: true
    ShowReadingTime: true

---

# Introduction

This project is a graphical interface to the [docx2pdf] module (https://pypi.org/project/docx2pdf/), which consists of converting docx files to pdf.

# Description
### A simple tool to find for an efficient use

Having to search for a site to convert words into PDF was too painful.
Today, I can in a few clicks 🖱️ overcome this problem.

![Illustration how to find Word2pdf](/Recherche-word2pdf.png)
As you can see, it is very easily accessible

### The interface

![The interface](/word2pdf-interface.png )
Granted, it's not the most *sexy* interface in the world

{{< encadres-markdown type="note" title="The idea is simple, I have 2 options open to me: " >}}
 - Convert ***a DOCX file*** to PDF
 - Convert ***all files in a folder*** that are DOCX to PDF
{{< /encadres-markdown >}}

![Process](/word2pdf-process.png )

Translated with www.DeepL.com/Translator (free version)