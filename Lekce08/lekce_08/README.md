# Tvořím web A–Z: lekce 08

<span>3. 11. 2020 | 18:00 - 20:00 | Praha</span>
Lekce 08 - pseudoelementy, animace, transformace
Tomáš Kazatel

---

# Dotazy k SuperAplikaci

- odpovídá @Tom.Kout

---

# Nebude nový úkol

---

# Podklady

[https://github.com/tvorimweb-2020-praha-podzim/lekce_08](https://github.com/tvorimweb-2020-praha-podzim/lekce_08)

---

# Calc()

- umožňuje vložit matematický výraz do CSS
- matematické operace +, -, *, /
- pořadí vykonávání pomocí dalších ( )

```css=
div { width: calc(100% / 3 - (2 * 1em)); }
```

---

# :first-child, :last-child

```css=
/* První potomek elementu */
div:first-child {}

/* Poslední potomek elementu */
div:last-child {}
```

---

# :nth-child

```css=
/* pravidlo platí pro druhou položku seznamu */
li:nth-child(2) {}

/* pravidlo platí pro každou třetí položku */
li:nth-child(3n) {}

/* jako předchozí, ale začíná se u druhé položky */
li:nth-child(3n + 2) {}
```

---

# ::before, ::after

```css=
div::before { content: 'Před'; }

div::after { content: 'Za'; }
```

```htmlmixed=
<div>
  Před
  <!-- Vše ostatní co bylo v divu předtím -->
  Za
</div>
```

---

# Co můžu použít v content

```css=
div::before { content: 'Text'; }

div::before { content: 'url(/cesta/k/obrazek.jpg)'; }

/* Nic, pro obrázková pozadí*/
div::before { content: ''; } 

div::before { content: "<h1>Toto nejde!</h1>"; }
```

---

# Transform ≠ Transition

- transform = změna tvaru elementu
- transition = animace přechodu mezi stavy elementu

---

# Transform 1/2

```css=
/* Zkosení */
.skew { transform: skew(-15deg); }

/* Otočení */
.rotate { transform: rotate(-15deg); }
```

note: 

- jendotka deg = úhel ve stupních 
- https://developer.mozilla.org/en-US/docs/Web/CSS/angle
---

# Transform 2/2

```css=
/* Posun */
.translate { transform: translate(0, 50%); }

/* Změna velikosti */
.scale { transform: scale(1.5); }
```

---

# Transition

```css=
button {
    background-color: blue;
    transition: 300ms;
}

button:hover {
    background-color: red;
}
```

---

# Transition - jednotlive vlatnosti 1/2

```css=
div {
    /* co se bude animovat */
    transition-property: margin, height, ...;
    
    /* jakým způsobem se bude animovat */
    transition-timing-function: ease | linear | ...;
}
```

note:

- https://css-tricks.com/almanac/properties/t/transition/

---

# Transition - jednotlive vlatnosti 2/2

```css=
div {
    /* jak dlouho bude animace probíhat */
    transition-duration: 500ms | 0.5s;
    
    /* jak dlouho se počká než začne průběh */
    transition-delay: 500ms | 0.5s;
}
```

---

# Transition - zkratka

```css=
element {
    transition:
        ([transition-property])
        [transition-duration]
        ([transition-timing-function])
        ([transition-delay]);
}
```

---

# Transition - příklad

```css=
div {
    margin-top: 100px;
    transition: margin-top 300ms ease 1s;
}

div:hover {
    margin-top: 200px;
}
```

note:

https://css-tricks.com/almanac/properties/t/transition-timing-function/

---












