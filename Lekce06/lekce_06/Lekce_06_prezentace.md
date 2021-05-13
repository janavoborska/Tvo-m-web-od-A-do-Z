---
tags: czechitas
lang: cs
slideOptions:
    transition: none
    theme: night
    margin: 0.05
    minScale: 0.1
    maxScale: 5
    width: 2560
    height: 1600
title: Lekce 06 | Tvořím web A–Z
---

{%hackmd anYwyN--TziyASUWcqP-Gw %}

# Tvořím web A–Z: lekce 06

<span>20. 10. 2020 | 18:00 - 20:00 | Praha</span>
Lekce 06 - Layout, media-queries
Tomáš Kazatel

---

# Podklady

[https://github.com/tvorimweb-2020-praha-podzim/lekce_06](https://github.com/tvorimweb-2020-praha-podzim/lekce_06)

---

# Doplnění z minula

- align-items
- align-self
- flex-basis (row) = width
- flex-basis (column) = height
- flex-direction: column - vlastnosti justify-content a align-items opačně

---

# Fixní layout

- již dlouho překonaný styl
- fixní = statický
- většina elementů je v px
- elementy se po stránce nepohybují
- nezáleží na velikosti obrazovky

---

<img src="https://miro.medium.com/max/2000/1*dUZudP2xfPLzMiw5L8ieTQ.gif" style="max-height: 180vh;" />

---

# Fluidní layout

- stále hodně používaný i když překonaný
- většina velikostí je zapsána v %
- elementy se po stránce nepohybují
- záleží na velikosti obrazovky
- není vhodný pro mobilní zařízení

---

<img src="https://miro.medium.com/max/2000/1*Hul4o5D73lpzVeVTk2Cuag.gif" style="max-height: 180vh;" />

---

# Adaptivní layout

- před media queries asi nejpoužívanější
- pro každou velikost definovaná verze
- elementy už se na stránce pohybují
- záleží na velikosti obrazovky
- zbytečný kód pro každou verzi

---

<img src="https://miro.medium.com/max/2000/1*LP6jyJPC17EVOk8nKEHYzg.gif" style="max-height: 180vh;" />

---

# Responzivní layout

- bere si to nejlepší z fluidního a adaptivního
- používají se breakpointy media-queries
- rozděluje rozlišení do rozmezí
- elementy se přesouvají, mení pozici i velikost
- minimalizuje zdrojový kód

---

<img src="https://miro.medium.com/max/2000/1*jGg5Y0CIZSGSTDTabsarbQ.gif" style="max-height: 180vh;" />

---

# Mobile first

<img src="https://content.altexsoft.com/media/2017/04/mobile-first-design-1024x404.png" style="max-height: 130vh;" />

---

# Media queries / breakpointy

<img src="https://www.vzhurudolu.cz/prirucka-content/dist/images/original/media-query.jpg" style="max-height: 130vh;" />

---

# Media queries / breakpointy

- typ média - screen, all, print, only
- logické operátory - and, (or = ,)
- vlastnost média - min-width, max-width, atd.
- hodnota zlomu - px, em

---

# Nejpoužívanější queries

- @media screen and (min-width: 1025px){...}
- @media screen and (min-width: 768px) and (max-width: 1025px){...}
- @media screen and (max-width: 767px){...}

---

# Jdeme kódit!!!

---

# Třetí povinný úkol

[https://classroom.github.com/a/apsLH2Xi](https://classroom.github.com/a/apsLH2Xi)

---








