# Tvořím web A–Z: lekce 04

<span>5. 10. 2020 | 18:00 - 20:00 | Praha</span>
Lekce 04 - Flexbox
Tomáš Kazatel

---

# Co první povinný úkol?

---

# Stáhnout podklady

[https://github.com/tvorimweb-2020-praha-podzim/lekce_04](https://github.com/tvorimweb-2020-praha-podzim/lekce_04)

---

# Trocha historie

1. pozicování pomocí tabulek
2. float, position, display
3. flexbox
4. css grid 

---

# Flexbox

- jednosměrný design
- rozlišujeme flex <b>kontejner</b> a flex <b>položky</b>
- rozlišujeme hlavní a vedlejší osu
- směry os se ale mohou měnit
- skvělý zdroj: [https://css-tricks.com/snippets/css/a-guide-to-flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox)

---

# Kontejner vs položka

![container](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)
![položka](https://css-tricks.com/wp-content/uploads/2018/10/02-items.svg)

---

# Jak na to

```css
.kontejner {
    display: flex;
}

```

---

# Rosteme (flex-grow)

![flex-grow](https://css-tricks.com/wp-content/uploads/2018/10/flex-grow.svg)

```css
/* default: 0 */

.jednicka {
    flex-grow: 1;
}

.dvojka {
    flex-grow: 2;
}

```

---

# Zmenšujeme se (flex-shrink)

```css
/* default: 1 */

.polozka {
    flex-shrink: 3; 
}

```

---

# Zkratka pro položky (flex)

```css
/* flex: <flex-grow> <flex-shrink> <flex-basis> */

/* default: 0 1 auto */

.polozka {
    flex: 1 0 200px;
}

```

---

# Zarovnání položek

```css
/* justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | ...*/

/* default: flex-start */

.kontejner {
   justify-content: center;
}

```

- [justify-content](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)

---

# Zalomení

![flex-wrap](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)

```css
/* flex-wrap: nowrap | wrap | wrap-reverse; */

/* default: nowrap */

.kontejner {
    flex-wrap: wrap;
}

```

---

# Pořadí

![order](https://svgshare.com/i/QJH.svg)

```css
/* default: 0 */

.polozka {
    order: 5;
}

```

---

# Příklad

- složka <code>02_cviceni</code>


---

# Druhý povinný úkol

[https://classroom.github.com/a/eHB236TU](https://classroom.github.com/a/eHB236TU)

---








