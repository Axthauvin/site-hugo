---
title: "Cacher du texte dans du texte"
date: 2021-11-04T22:35:57Z
draft: false

author: ["Axel Thauvin"]

cover:
    image: "https://delante.co/wp-content/uploads/2019/11/hidden-text-definicja.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "Illustration"
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

{{< encadres type="" titre="❔Where can you find the project" >}}
  Projet is currently hosted on <a href="https://cacherdutexte.github.io">https://cacherdutexte.github.io</a>
{{< /encadres >}}


###  How did I hid text in text 
This is a bitwise way of hiding text within text.
Let's imagine the string :
```
Hacker
```
That I want to hide in the message:
```
Hello, I am Axel Thauvin
``` 

- First, we get the **decimal representation in the UTF-8 table** of each character in the `Hacker` string

  *Here is the decimal representation of the first 127 characters in an array (also called ASCII array):*
  ![Tableau ascii](https://github.com/Axthauvin/cacher-du-texte-dans-du-texte/blob/main/images/UTF8-TABLE.png?raw=true)


For the example, we will take the character `H`.
Here, its decimal representation is ***72*** (base 10).

- Then we will convert this number to base 6 on 4 'bits'
  # Why ?
  If we encode the letters in base 6 on 4 bits, we will have the maximum representation of `5555` -> that is 6<sup>4</sup> -> 1296 : *which is the maximum value we can use in this table*
  
  In fact we have 5 **invisible characters** which will correspond to the digits of these bits, which we will *hide* in our text.
  - *For the 0 there is no hidden character*.
  - *For 1 it is the unicode character `\u200C`*
  - *For 2 it is the unicode character `\u200D`*
  - *For 3 it is the unicode character `\u200E`*
  - *For 4 it is the unicode character `\u200F`*
  - *For 5 it is the unicode character `\u034F`*
  
  # Example with `H`
  
  Here the decimal representation of `H` is ***72***.
  Its 4-bit *base-6* representation is `0200`.
  
  I will therefore :
  - Not add a character for the 1st bit (because it is 0)
  - Add the character `\u200D` for the 2nd bit (because it is 2)
  - Not add a character for the 3rd bit (because it is 0)
   - Do not add a character for the 4th bit (because it is 0)
  
  ***Let's go back to the original string***.
  I have `Hello, I am Axel Thauvin`.
  So I'll write : **He`\u200D`ll** just for the H
  
  ***And I do the same with all the characters in `Hacker`.***
  Which gives me: 
  `He‍‍llo‍,‏‍‌ ‏‍I‏‌‎ a‍‍͏m͏‏ ‍‎‏A͏x‍‎e‌͏l͏ T‍h‏a͏uv‎i‌n` (generated with my program, you can try it on my website)
  
  ***Here is the result:***
  
  ![Image gif](https://github.com/Axthauvin/cacher-du-texte-dans-du-texte/raw/main/images/VideoIllustration.gif)