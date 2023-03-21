# CSS3 tanfolyam

https://w3.org/style/css
https://e-learning.training360.com/courses/take/A-CSS-nyelv-alapjai/lessons/39193959-a-fejlesztokornyezet
https://e-learning.training360.com/courses/take/css3-halado/lessons/17161602-css3-szabvanyok

## Weboldalak fő összetevői:
- HTML5: Weboldal struktúrája, tartalma, váza (szövegek, képek, linkek stb.) stílusjegyek nélkül
- CSS3: Weboldal design/stílus jegyek a HTML építőkockák számára (szövegméret, háttérszín, betűstílus stb.)
- JS (JavaScript [jávaszkript]): Felhasználói interakciók (pl. gombra kattintásra végrehajtódó esemény)

- A weboldalak megjelenéséért, stílusjegyeiért és dizájnjáért felelős leírónyelv a CSS [szíeszesz].
-  Cascading Style Sheet [kászkáding sztájl sítsz], egymásba ágyazott (lépcsőzetes) stíluslapok
- HTML web dokumentumok szabványos stíluslapja (leíró mechanizmusa) a weboldalak megjelenésének meghatározására (ez egyes elemekre vonatkozó betűtípusok, színek, térközök stb. megadásával)
- egyszerű szöveges fájl, a kiterjesztése .css (pl. _styles.css_)
- a HTML oldal <head> szekciójában hivatkozunk rá az első megjeleníthető elem előtt (pl. <link rel="stylesheet" href="css/style.css">):

## Fejlesztői környezet:
- VSCode [véeskód]: ingyenesen letölthető
  - Live Server Extension
- JSBin [jéesbin] böngészőben futó weboldal szerkesztői környezet, egyszerű HTML, CSS és JavaScript kódrészletek vizsgálatára és tesztelésére (https://jsbin.com/?html,output)
- Kód vizsgálata: Böngészőben az Inspect helyi menüt kiválasztva (F12 billentyű) megjelenő kis ablakban az Element (HTML tartalom) és Styles (CSS tartalom) fülek alatt

## CSS komment
- A böngésző figyelmen kívül hagyja a /* … */ módon határolt tartalmat

## Link HTML (content) and CSS (design) in priority order
1. [Inline CSS](#inline-css) - unique style for one element
1. [Internal CSS](#internal-css) - unique style for one HTML page
1. [External CSS](#external-css) - common styles for HTML pages

### Inline CSS
- Inline CSS [inlájn szíeszesz] esetén minden elem esetén egyedileg kell beállítani a stílust, nincsenek újrahasználható stílusjegyek, boilerplate (feleslegesen ismétlődő elemeket tartalmazó) és nehezen olvasható kódot eredményez
- html elem style attribútumának értékeként megadott property: value; (tulajdonság: érték;) párokként sorolhatjuk fel a saját stílusszabályainkat:
  <tag style=property: value; property: value …>
  pl.:
    <body>
    …
      <h3 style="color: blue; font-size: 22px;">
    …
    </body>

### Internal CSS
- Internal CSS [internál szíeszesz]: növeli az olvashatóságot, azonos elemekre elegendő egy helyen megadni a stílusszabályokat, de ezek az egyedi stílusjegyek csak az adott HTML oldal elemeire vonatkoznak, más oldalakon nem használhatók 
- a HTML oldal <head>…</head> szekciójában, <style>…</style> tag-ek között szelektorral azonosított elemekre vonatkozóan {…} kapcsos zárójelek között felsorolt stílusszabályok
  pl.:
    <head>
    …
      <style>
        h3 {
          color: blue;
          font-size: 22px;
        }        
      </style>
    …
    </head>

### External CSS
- External CSS [externál szíeszesz]: HTML tartalom és dizájn különválasztás a CSS stílusszabályok külső fájlba szervezésével; ez a leggyakoribb, több HTML oldalon is felhasználható, könnyen módosítható, közös megoldás (akár több fejlesztő párhuzamosan is dolgozhat az egyes fájlokon). - Több CSS fájl és/vagy egyidőben internal és inline stílusmegadás esetén ütközés is előfordulhat (több, egymásnak ellentmondó szabály vonatkozhat egy elemere), ami nagyméretű fájlok esetén megnehezíti a hibakeresést és -javítást. Ilyenkor a legnagyobb precedenciával az inline (konkrétan az adott elemre vonatkozó), majd az internal (konkrétan az adott weboldalra vonatkozó) stílus rendelkezik.
- az internal CSS <style>…</style> tag-jai közötti stílusszabály-tartalom fájlba írása és erre a fájlra való hivatkozás (összekapcsolás) definiálása a HTML oldal <head>…</head> szekciójában, a <link> tag attribútumaként a CSS fájl referenciájának megadásával <link rel="stylesheet" href="…"> formában, pl.:
    <head>
    …
      <link rel="stylesheet" href="css/style.css">
    …
    </head>

```
<!-- index.html: -->
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/style.css">
    <title>Document</title>
  </head>
  <body>
  </body>
```

**HTML + CSS példakód external CSS használatával:**
/* css/style.css: */
  div {
  border: 1px solid grey;
  text-align: center;
}

<!-- index.html: -->
  <!DOCTYPE html>
    <html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width">
      <title>JS Bin</title>
      <link rel="stylesheet" href="css/style.css">
    </head>
    <body>
      <div>
       <h3>Title</h3>
       <button onclick=alert("Click!")>Click me</button>
     </div>
    </body>
  </html>

## CSS Box Model
- a box that wraps around every HTML element
  - margin: space between elements
  - border: space between margin and padding, part of the element
  - padding: space between border and content of the element
  - content: element content; text, image etc.

## CSS Selectors
Select element
- **id**: unique within a page, e.g. _#idname {…}_
- **class**: _.classname {…}_
- **element**: _tagname {…}_
- **universal**: selects all HTML elements on the page, e.g. _* {…}_
- **attribute**:
  - equality with an attribute: _tagname[attribute-name] {…}_
  - equality with an attribute and its value: _tagname[attribute-name="value"] {…}_
  - attribute start with a value: _tagname[attribute-name^="value"] {…}_
  - attribute end with a value: _tagname[attribute-name$="value"] {…}_
  - attribute contains a value: _tagname[attribute-name~="value"] {…}_
  - attribute contains a value or a value followed by a hyphen (-): _tagname[attribute-name|="value"] {…}_
  - attribute contains a value part: _tagname[attribute-name*="value"] {…}_
- **pseudo**:
  - class: _selector:pseudo-class {…}_
  - element: _selector::pseudo-element {…}_
- **combinator**: explains relationship between the selectors
  - descendant selector (space) for descendant elements (child, grandchild etc.) e.g. _div p {…}_
  - child selector (>) for children an element e.g. _div > p {…}_
  - adjacent sibling selector (+) sibling for directly after an element e.g. _div + p {…}_
  - general sibling selector (~) sibling for next after an element e.g. _div ~ p {…}` _
- **grouping**: _selector, selector, … {…}_

Pseudo Class|Description
-:|-
`selector:active`|_Selects the active element (e.g. link)_
`selector:checked`|Selects every checked element_
`selector:disabled`|_Selects every disabled element_
`selector:empty`|_Selects every element that has no children_
`selector:enabled`|_Selects every enabled element_
`selector:first-child`|_Selects every elements that is the first child of its parent_
`selector:first-of-type`|_Selects every element that is the first element of its parent_
`selector:focus`|_Selects element that has focus_
`selector:hover`|_Selects element on mouse over_
`selector:in-range`|_Selects elements with a value within a specified range_
`selector:invalid`|_Selects all elements with an invalid value_
`selector:lang(language-code)`|_Selects every element with a lang attribute value starting with language-code_
`selector:last-child`|_Selects every elements that is the last child of its parent_
`selector:last-of-type`|_Selects every element that is the last element of its parent_
`selector:link`|_Selects all unvisited links_
`:not(selector)`|_Selects every element that is not a selector element_
`selector:nth-child(n)`|_Selects every element that is the n. child of its parent_
`selector:nth-last-child(n)`|_Selects every element that is the second child of its parent, counting from the last child_
`selector:nth-last-of-type(n)`|_Selects every element that is the n. element of its parent, counting from the last child_
`selector:nth-of-type(n)`|_Selects every element that is the n. element of its parent_
`selector:only-of-type`|_Selects every element that is the only element of its parent_
`selector:only-child`|_Selects every element that is the only child of its parent_
`selector:optional`|_Selects elements with no "required" attribute_
`selector:out-of-range`|_Selects elements with a value outside a specified range_
`selector:read-only`|_Selects elements with a "readonly" attribute specified_
`selector:read-write`|_Selects elements with no "readonly" attribute_
`selector:required`|_Selects elements with a "required" attribute specified_
`:root`|_Selects the document's root element_
`#id:target`|_Selects the current active #id element (clicked on a URL containing that anchor name)_
`selector:valid`|_Selects all elements with a valid value_
`selector:visited`|_Selects all visited (links)_

Pseudo Element|Description
-:|-
`selector::after`|_Insert something after the content of each element_
`selector::before`|_Insert something before the content of each element_
`selector::first-letter`|_Selects the first letter of each element's content_
`selector::first-line`|_Selects the first line of each element's content_
`::marker`|_Selects the markers of list items_
`selector::selection`|_Selects the portion of an element that is selected by a user_

## Floating igazítások

- `box-sizing` - elem igazításának beállítása
- minden elemre vonatkozik, hogy a `padding` és a `border` szélessége nem növeli az elem méretét:
```
    * { 
        box-sizing: border-box;
      }
```
- azonos osztályba tartozó elemek formázása (`class="..."` attribútum) osztály szelektorral (`.`), balra igazítva jelenjen meg minden, az adott osztályba tartozó elem és az oldalszélesség 1/3-át foglalja el, 5 pixellel befelé csökkentett méretű tartalommal (a minden elemre érvényes `box-sizing: border-box` miatt):
```
    .img-container {
        float: left;
        width: 33.3%
        padding: 5px; 
    }
```
- az adott osztályba tartozó elem háttérszíne (`background-color`) aqua legyen:
```
    .clearfix {
        background-color: aqua;
    }    
```
- az adott osztályba tartozó blokkszintű elem után (`::after`) másik sorban jelenjen meg a következő elem: 
```
    .clearfix::after {
        content: "";
        clear:both;
        display:table;  
    }
```

## Position

- Megmondja, hogy egy elem az oldalon hová legyen pozicionálva
  - `position: static` [sztetik] (alapértelmezett értéke a statikus pozicionálás, amikor az elem pozícióját a többi elem határozza meg az oldalon (az előtte lévő elem után következik)
  - `position: relative` [relatív] (az elem eltolása valamilyen irányba az eredeti pozíciójához képest (top, bottom, left, right eltolás adható meg)
  - `position: fixed` [fikszd] (az elem pozíciója fixen megadható a top, bottom, left, right attribútumokkal ill. azok egy részével)
  - `position: absolute` [abszolút](ahhoz a szülő elemhez igazítja magát, ami abszolút, relatív vagy fixed
  - `position: sticky` [sztiki] (top: 0 attribútummal pl. menüknél használatos, scroll-ozható oldalon egészen addig a több tartalommal együtt mozog felfelé, amíg nem ér az oldal tetejére, de onnan nem tűnik el, mint a kifutó tartalom, hanem ott marad és visszafelé görgetéskor akkor indul el lefelé, amikor az eredeti pozíciója újra megjelenik az oldal látható részén)

**Pozicionálás példa:**
```
/* css/style.css: */
  .static {
    position: static;
    border: 3px solid #73AD21;
  }
  .relative {
    position: relative;
    left: 30px;
    border: 3px solid #2123ad;
  }
  .fixed {
    position: fixed;
    left: 100px;
    right: 100px;
    top: auto;
    bottom: 0;
    border: 3px solid black;
  }
  .absolute {
    position: absolute;
    top: 50px;
    left: 100px;
    width: 200px;
    border: yellow;
  }
  div.sticky {
    position: sticky;
    top: 0;
    background-color: brown;
    color: white;
  }

<!-- index.html: -->
  ...
  <body>
    <div class="static">This is a static div element</div>
    <div class="relative">This is a 30px left relative div element</div>
    <div class="fixed">This is a fixed div element</div>
    <div class="relative">This is a parent to an absolute element
      <div class="absolute">This is an absolute elment</div>
    </div>
    <div class="sticky">This is a sticky element</div>
    <div style="padding-bottom: 2000px;">
      <pre>
        a
        b
        c
        ...
        x
        y
        z
      </pre>
    </div>
  </body>
  ...
```

## Haladó mértékegységek

- A böngésző alap szövegméret-beállítása 12 pixel
- `em`: soremelés mértéke az alapértelmezett (vagy szülő elembeli) betűmérethez képest relatívan megadva, pl. line-height: 2em (a soremelés mértéke a betűméret 2x-ese, alapértelmezett betűméret esetén 24 pixel)
- `vh`: viewport high, az elemnek a böngészőablak méretéhez viszonyított magassága %-ban megadva (pl. width: 33vw;)
- `vw`: viewport width, az elemnek a böngészőablak méretéhez viszonyított szélessége %-ban megadva (pl. height: 20 vh;)

## Pszeudo-elemek
- CSS elemekhez kapcsolódnak, a böngésző hozza őket létre automatikusan
  - `::after` [after]: az elem után
  - `::before` [bifór]: az elem előtt
  - `::checked` [csekd]: a checkbox be van jelölve (ki van pipálva)
 
**Custom checkbox példa:**
```
/* css/style.css: pszeudo elemek gyakorlása (gomb) */
  .tgl {
    display: none;
  }
  .tgl, .tgl:after, .tgl + .tgl-btn, .tgl *, .tgl *:after  {
    box-sizing: border-box;
  }
  .tgl + .tgl-btn {
    outline: 0;
    display: block;
    width: 4em;
    height: 2em;
    position: relative;    
    cursor: pointer;
    user-select: none;
  }
  .tgl + .tgl-btn:after {
    display: block;
    position: relative;
    content: "";
    width: 50%;
    height: 100%;
  }
  .tgl + .tgl-btn:after {
    left: 0;
  }
  .tgl:checked + .tgl-btn:after {
    left: 50%;
  }
  .tgl-btn {
    background-color: #f0f0f0;
    border-radius: 2em;
    padding: 2px;
  }
  .tgl + .tgl-btn:after {
    border-radius: 50%;
    background-color: #fff;
  }
  .tgl:checked + .tgl-btn {
    background-color: #9fd6ae;
  }

<!-- index.html: -->
  ...
  <body>
    <h2>Custom checkbox</h2>
      <ul class="tg-list">
        <li class="tg-list-item">
          <input class="tgl tgl-light" id="cb1" type="checkbox" checked>
          <label class="tgl-btn" for="cb1">
          </label>
        </li>
      </ul>
  </body>
  ...
```

- Az \<input id="xyz">-hoz kapcsolódó \<label>-t \<label for="xyz"> formában hozhatunk létre, ilyenkor ha a \<label>-re kattintunk az olyan, mintha az \<input>-ra kattintottunk volna.
- A példában a tgl a toggle [tágl] (váltó) rövidítése
- Az \<input type="checkbox" checked> a checkbox elem bekapcsolt állapotát jelenti
- a css-ben a .tgl + a for-t jelenti (a tgl osztályú input-hoz tartozó label-t)
- display: none; - az elem elrejtése
- box-sizing: border-box; - a margin és a padding nem adódik hozzá a mérethez, hanem beleszámít
- outline: 0; - nincs kiemelés
- width: 4em; - követi a beállított betűméretet, ahozz képest méretezzük, igazodik a szülő elem font-size méretéhez
- position: relative; - az elem mozgatható, ha szükséges
- cursor: pointer; - egy kis kéz jelenik meg, ha az elem fölé visszük az egeret (ebből látszik, hogy rá lehet kattintani)
- user-select: none; - ha húzzuk az egeret, az elem nem jelölhető ki húzással (nem lesz kék háttere)
- content: ""; - bár a CSS megjelenés meghatározására való, a pszeudo elemekhez tartalom is definiálható
- width: 50%; - az elem fele olyan széles lesz, mint a befogadó elem (itt a label)
- width: 100%; - az elem ugyanolyan magas lesz, mint a befogadó elem (itt a label)
- left: 0; - az adott elem alapértelmezés szerint a szülő elem bal oldalán helyezkedik el
- border-radius: 2em; - elem sarkainak lekerekítése
- Kezelése JavaScript-ben (Google Chrome F12 fejlesztői panel Console):
```
    > const input = document.querySelector('input')
    < undefined
    > input.checked 
    < false
    > input.checked = true
    < true
```

## Display haladó szinten

- Azt a box-ot módosítja, amiben az elem megjelenik (virtuálisan a böngészőben minden elemnek van egy doboza, amiben megjelenik és ennek a méreteit tudjuk módosítani css beállításokkal)
- Leggyakoribb beállításai:
  - `display:block` [diszpléj blokk] (a blokk szintű elemek teljes szélességben kitöltik a rendelkezésükre álló helyet, ezért a width beállítás itt nem érvényesül)
  - `display:inline` [diszpléj inlájn] (a width-et és a height-et ill. a felső és az alsó margót figyelmen kívül hagyja; de a paddingot és mivel a line-height a szövegre vonatkozik, annak az értékét is figyelembe veszi)
  - `display:inline-block` (a block és az inline előnyeit ötvözi, a width és a height is beállítható a böngésző számára)

```
/* css/style.css: */
  div {
    background-color: gold;
    margin: 0.5em;
    border: 0.5em;
    padding: 0.5em;
    width: 2em;
    height: 2em;
    cursor: pointer;
  }
  .block {
    display: block; 
  }
  .inline {
    display: inline; 
  }
  .inline-block {
    display: inline-block; 
  }

<!-- index.html: -->
  ...
  <body>
    <h1>Display css example</h1>
    <p>display: block</p>
    <div class="block"></div>
    <div class="block"></div>
    <div class="block"></div>
    <p>display: inline</p>
    <div class="inline"></div>
    <div class="inline"></div>
    <div class="inline"></div>
    <p>display: inline-block</p>
    <div class="inline-block"></div>
    <div class="inline-block"></div>
    <div class="inline-block"></div>
  </body>
  ...
```

- text-align: center; - középre igazított szöveg
- color: gold; - aranyszínű elem
- font-size: 2em; - 2x-es betűméret az aktuálishoz képest (a szülőelem betűméretéhez képest)
- text-shadow: 0 0 2px #ff0000; - szövegárnyék
- width: 2em; - elem szélessége
- line-height: 2em; - elem sormagassága

## Sarkok lekerekítése

- background: transparent - átlátszó háttér
- color: inherit,  font: inherit; -  a gomb a szülő elemtől örökli a színét és a betűtípusát
- button:focus; - a focus pszeudóosztállyal állíthatjuk be, mi történjen, ha fókuszba kerül a gomb
- button-inner; - a gomb belső része
- align-items: center; - elemek középre igazítása
- border: 2px solid transparent; - a keret 2 pixel vastag, folytonos vonal és átlátszó
- border-radius: 99em; - sarkok lekerekítése (lehetőleg félkör legyen, extrém nagy betűméretnél is; ha kisebbet adnánk meg a betűméretnél, csak a sarkok lennének lekerekítve, ha nagyobbat, a lekerekítés akkor is félkör alakú lesz)
- color: #fff: fehér szín
- font-family: sans-serif; - talp nélküli betűcsalád
- font-weight: 600; - közepesen vastag betű (100-tól 900-ig módosítható, a nagyobb szám nagyobb vastagságot jelent)
- min-width: 2.5em; - minimális szélesség
- .button:focus; - ha fókuszt kap a gomb
- .button:hover; - ha az egérmutató a gomb fölött van
- .button:active; - ha a gomb aktív

```
/* css/style.css: */
  /* CSS kitisztázás a button számára: */
  .button {
    background: transparent;
    border: 0;
    border-radius: unset;
    color: inherit;
    display: inline-block;
    font: inherit;
    height: auto;
    line-height: 1;
    margin: 0;
    padding: 0;
    position: relative;
    text-align: center;
    text-decoration: none;
    user-select: none;
  }
  .button:focus {
    outline: none;
  }
  .button-inner {
    align-items: center;
    background: #456bd9;
    border: 2px solid transparent;
    border-radius: 99em;
    color: #fff;
    display: flex;
    font-family: sans-serif;
    font-weight: 600;
    height: 2.5em;
    min-width: 2.5em;
    padding: 0 1em;
    position: relative;
  }
  .button:focus .button-inner {
    border-color: #fff;
    box-shadow: 0 0 0 2px #456bd9;    
  }
  .button:hover .button-inner {
    filter:brightness(1.1);
  }
  .button:active .button-inner {
    filter:brightness(0.9);
  }
  .badge {
    align-items: center;
    background: crimson;
    border: 2px solid white;
    border-radius: 99em;
    color: white;
    display: flex;
    font-size: 0.7em;
    font-weight: 600;
    height: 1.44em;
    justify-content: center;
    line-height: 1;
    min-width: 1.44em;
    position: absolute;
    right: -2px;
    top: -2px;
  }

<!-- index.html: -->
  ...
  <body>
    <button class="button">
      <span class="button-inner">
        Messages
      </span>
      <span class="badge">
        4
      </span>
    </button>
  </body>
  ...
```

## Reszponzív képek
- Ha változik a mérete a kijelzőnek (pl. elfordítják a mobiltelefont) vagy tabletre ill. nagyfelbontású kijelzőre eltérő képeket szeretnénk megjeleníteni, CSS3 előtt pl. a kép %-os méretének beállításával volt lehetőség a képméret skálázására.
- CSS3-tól egy képnek több forrás is megadható és pl. a beállított kijelző szélességtől függően az adott kijelzőmérethez rendelt forrásból kerül a kép betöltésre (pl. 3 képforrás esetén, ha az első kettőhöz 480px ill. 800px kijelző-szélesség van beállítva, 480px szélességű kijelzőnél csak az első, 481-800px szélesség esetén a második, ennél nagyobb kijelző esetén a harmadik forrásból kerül a kép betöltésre)
- Különböző forrásokból tehát különböző méretű képek is betölthetők, ami az adatforgalom menedzselésére is lehetőséget nyújt (pl. kisebb adatforgalom generálható mobiltelefon esetén, ha a kép kisebb felbontású változatát jelenítjük meg)

```
<!-- index.html: -->
  ...
  <body>
    <picture>
      <source srcset="http://.../roses-small.webp" media="(max-width: 480px)">        
      <source srcset="http://.../roses-medium.webp" media="(max-width: 800px)">        
      <source srcset="http://.../roses-big.webp">        
      <img src="" alt="Roses">
    </picture>
  </body>
  ...
```

## Hátterek beállítása
- Gyakran előfordul, hogy egy HTML oldalnak vagy annak bizonyos elemeihez (pl. div-ek) háttérképet kell beállítanunk. 
- `background-color: white;` háttér színe
- `background-image: url(../img/roses-small.webp);` háttérkép, pl. url függvénnyel adható meg a forrása
- `background-repeat: no-repeat;` ismétlődjön-e a háttérkép (mozaikszerűen kitöltve a rendelkezésére álló helyet, ha kisebb; ha nagyobb vagy nem kérünk ismétlődést, a bal felső saroktól teszi be)
- `background-attachment: fixed;` (alapértelmezett illesztés)
- `background-position: left top;` (alapértelmezett elhelyezés)
- Shorthand (rövid, összefoglaló beállítás, a paraméterek a fenti sorrendben adandók meg szóközzel elválasztva):
    `background: white url(../img/roses-small.webp) no-repeat fixed left top;`

```
/* css/style.css: */
body {
/*
    background-color: white;
    background-image: url(../img/roses-small.webp);
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: left top;
  Shorthand:    
*/
  background: white url(../img/roses-small.webp) no-repeat fixed left top; 
}
```

## Színátmenetek
- CSS3-ban lehetőség van színátmenetek létrehozására
- Beállítható, hogy honnan, hová és milyen átmenettel változzon egy szín (a background-image használatával több szín és azok súlyozása is megadható %-ban)
- `linear-gradient()`: folyamatos színátmenet, paraméterei a forrás- és a célszín ill. a színátmenet iránya fokban megadva (deg) 
- `radial-gradient()`: belülről kifelé, körökörös színátmenet (itt a fok nem adható meg, mert nincs értelme)
- `-webkit-text-fill-color`: transparent; az elem, amihez színátmenetet hozunk létre, legyen átlátszó
- `background-clip: text;` a háttér csatolási módja az elemhez, amihez színátmenetet hozunk létre (itt csak a szöveg jelenik meg a beállított színátmenettel)
- `-webkit-background-clip: text;` webkit alapú böngészőknél ezt a megjelenítési módot prefixálnunk kell (bizonyos böngészők csak akkor támogatják a különleges megjelenítést, ha a saját prefixük be van állítva hozzá, natív támogatás esetén elhagyható)

```
  /* css/style.css: */
  .gradient {
    font-size: 72px;
    background: -webkit-linear-gradient(30deg, red 0%, yellow 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  <!-- index.html: -->
  ...
  <body>
    <b><span class="gradient">GRADIENT TEXT</span></b>
  </body>
  ...  
```

## Árnyékok
- CSS3-ban a különféle HTML elemekez ill. szövegekhez árnyék is beállítható.
- Egy elemhez a paramétereket vesszővel elválasztva egymástól több árnyék is megadható
- Elem árnyékának beállítása: `box-shadow`, a paraméterei sorrendben:
  - `h-offset`: árnyék vízszintes irányú eltolása az elemhez képest (balról jobbra értendő)
  - `v-offset`: árnyék függőleges irányú eltolása az elemhez képest (fentről lefelé értendő)
  - `blur`: árnyék elmosódása
  - `spread`: az árnyék további kiterjedése
  - `color`: árnyék színe (rgba() függvénnyel az árnyék átlátszósága is megadható)
- Szöveg árnyékának beállítása: `text-shadow`
  - `h-offset`: árnyék vízszintes irányú eltolása az elemhez képest (balról jobbra értendő)
  - `v-offset`: árnyék függőleges irányú eltolása az elemhez képest (fentről lefelé értendő)
  - `blur`: árnyék rádiusza (szöveg körbefuttatása)
  - `color`: árnyék színe (rgba() függvénnyel az árnyék átlátszósága is megadható)

```
/* css/style.css: */
  div.card {
    width: 300px;
    box-shadow: 4px 4px 8px 0 rgba(0,0,0,0.3);
  }
  img {
    max-width: 100%;
    max-height: 100%;
  }
  div.text p {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1.5em;
    color: gray;
    text-align: center;
    text-shadow: 1px 1px 5px rgba(255,0,0,0.5);
  }

<!-- index.html: -->
  ...
  <body>
    <h1>Test page</h1>
    <div class="card">
      <img src="./img/roses-small.webp" alt="roses">
      <div class="text">
        <p>Nice roses</p>
      </div>
    </div>
  </body>
  ...  
```

## Betűhatások
- Szöveg-effektusok (text-effects)
- `white-space: nowrap;` az üres karaktereknél nem vágja el, nem folytatja új sorban a szöveget (normal esetén,a mi az alapértelmezés, tördeli)
- `overflow: hidden;` el lesz rejtve a túlcsorduló szövegrész
- `text-overflow: clip|ellipsis` túl hosszú szöveg végének levágása (az ellipsis előbb ...-ot ír)
-` word-break: keep-all;` nem töri el a szövegben a hosszú szavakat, ha a rendelkezésre álló sor vagy szövegterület végére ér, még akkor sem, ha nem fér ki a szó a sorban
- `word-break: break-all;` eltöri a szövegben a hosszú szavakat, ha a rendelkezésre álló sor vagy szövegterület végére ér
- `writing-mode: horizontal-tb;` ez a default írásmód, vízszintesen és balról jobbra
- `writing-mode: vertical-lr|vertical-rl;` függőleges írásmód, fentről lefelé

```
/* css/style.css: */
  .to-clip {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: clip;
  }
  .to-ellipsis {
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .wb-keep-all {
    word-break: keep-all;
  }
  .wb-break-all {
    word-break: break-all;
  }
  .wm-horizontal {
    writing-mode: horizontal-tb;
  }
  .wm-vertical {
    writing-mode: vertical-lr;
  }

<!-- index.html: -->
  ...
  <body>
    <h1>Text effects</h1>
    <p>This paragraph contains a long text that will fit in the box.</p>
    <h3>text-overflow: clip </h3>
    <p class="to-clip">This paragraph contains a long text that will not fit in the box.</p>
    <h3>text-overflow: ellipsis </h3>
    <p class="to-ellipsis">This paragraph contains a long text that will not fit in the box.</p>    
    <h3>word-break: keep-all</h3>
    <p class="wb-keep-all">This paragraph contains a long text with a veryveryveryveryveryverylongworld that will not fit in the box.</p>    
    <h3>word-break: break-all</h3>
    <p class="wb-break-all">This paragraph contains a long text with a veryveryveryveryveryverylongworld that will fit in the box.</p>    
    <h3>writing modes</h3>
    <p class="wm-horizontal">This paragraph contains horizontal and <span class="wm-vertical">vertical</span> texts.</p>
  </body>
  ...  
```

## Transzformációk - 2D átalakítások
- alakzat 2 dimenziós transzformációja (mozgatása, nyújtása, méretezése, torzítása, skáklázása, forgatása) függvényekkel lehetséges
- a böngésző számára a transzformáció ellenére az elem olyan, mintha az eredeti helyén és méretében maradt volna, a többi elem helyzetét az elem transzformációja nem módosítja (így akár rá is csúszhat a transzformált elem egy másik elemre)
- `transform: translate(x-offset, y-offset)`: eltolja az elemet az eredeti helyéről, az x ill. y irányú relatív elmozdulást kell megadni
- `-ms-transform: translate(x-offset, y-offset)`: az előbbi transzformáció IE9 böngészővel működő változata
- `translateX()`, `translateY()`: elmozdítás csak az egyik dimenzióban
- `rotate()`: az elforgatás szögét kell megadni, az óramutató járásával megegyező irányban
- `scale()`: méretezés (skálázás) x ill. y kordináta viszonylatában, itt a szorzót (arányszámot) kell megadni az eredeti 1x-hez képest; kicsinyítés vagy nagítás is lehetséges
- `scaleX()`, `scaleY()`: skálázás csak az egyik koordináta esetén (a másik 1x marad)
- `skew()`: torzítás (nyújtás, zsugorítás) X ill. Y koordináta arányszámának megadásával, fokban
- `matrix()`: ezzel a `translate()`, `scale()` és a `skew()` egyszerre állítható: `matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY())` paramétersorrendben

```
/* css/style.css: */
  div {
    width: 50px;
    height: 50px;
    border: 1px solid black;
    box-shadow: 0 0 5px;
    background-color: yellow;
  }
  div:not(#parent) {
    background-color: brown;
  }
  .translate {
    -ms-transform: translate(50px, 10px);
    transform: translate(50px, 10px);
  }
  .rotate {
    transform: rotate(20deg);
  }
  .scale {
    transform: scale(0.5, 0.75);
  }
  .skew {
    transform: skew(10deg, 30deg);
  }
  .matrix {
    transform: matrix(0.5, 0.25, 0.1, 0.75, 50, 10);
  }

<!-- index.html: -->
  ...
  <body>
    <h1>2D transformations</h1>
    <h3>translate:</h3>
    <div id="parent">
        <div class="translate"></div>
    </div>
    <h3>rotate:</h3>
    <div id="parent">
        <div class="rotate"></div>
    </div>
    <h3>scale:</h3>
    <div id="parent">
        <div class="scale"></div>
    </div>
    <h3>skew:</h3>
    <div id="parent">
        <div class="skew"></div>
    </div>
    <h3>matrix:</h3>
    <div id="parent">
        <div class="matrix"></div>
    </div>
  </body>
  ...  
```

## Transzformációk - 3D átalakítások
- A már megismert 2 dimenzió (x és y tengely) bővül a z tengellyel, ami mélységggel bővíti az elem koordinátáit
- `translate3d()`: https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/translate3d
- `rotate3d()`: https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate3d
- `scale3d()`: https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/scale3d
- `matrix3d()`: https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/matrix3d

## Átmenetek
- Egy elem méretének, pozíciójának, színének stb. változtatása különféle átmenetekkel is megvalósítható.
- transition: megadjuk, hogy a változás mennyi idő alatt menjen végbe. Legegyszerűbb egy osztály megadásával az adott elemnek, ami a változásokat tartalmazza, majd beállítjuk, ez az elem legyen az elem új osztálya (pl. JavaScript kód segítségével, kattintásra)
- transition: all; esetén minden animálható módosításnál a beállított ideig tart az átmenet
- időgörbe is megadható (pl. ease-in-out lassan kezdődik és lassan fejeződik be az átmenet és közben gyorsabb)

```
/* css/style.css: */
  div {
    width: 50px;
    height: 50px;
    border: 1px solid black;
    box-shadow: 0 0 5px;
    background-color: yellow;
    color: white;
    text-align: center;
  }
  div:not(#parent) {
    background-color: brown;
  }
  .transition:hover {
    transition: all 3s ease-in-out;
    transform: translate(50px, 10px) rotate(180deg) scale(2, 2);
  }

<!-- index.html: -->
  ...
  <body>
    <h1>Transition</h1>
    <div id="parent">
        <div class="transition">Hover me</div>
    </div>
  </body>
  ...  
```

## Animációk
- Elam animációja CSS3 előtt Flash ill. JavaScript segítségével volt megvalósítható
- position: relative|absolute; paraméterrel lehetséges az animáció
- nem minden tulajdonság animálható, csak amiben lehetséges az átmenet egyik állapotból a másikba (pl. a display tulajdonságban nem)
- egyszerre több tulajdonság is animálható
- @keyframes animated_element_name: az animáció kulcskockájáának a neve, az idő %-ával jelezhető melyik fázisban miként működjön az animáció
- animation: animated_element_name duration timing-function delay iteration-count direction fill-mode
- 0%-nál és 100%-nál megegyező infinite animáció folyamatosan ismétlődni fog
- ha egy tulajdonságot módosítunk, minden animációs fázisban szerepeltetni kell a módosított állapotot (még akkor is, ha ott nem módosítjuk), különben a tulajdonság kiindulási értékét (amilyen az elem 0%-os animációs állapotában volt) veszi a böngésző alapul

```
/* css/style.css: */
  div {
    width: 50px;
    height: 50px;
    border: 1px solid black;
    box-shadow: 0 0 5px;
    background-color: brown;
  }
  #animated_div {
    position: relative;
    animation: animated_div 3s infinite;
  }
  @keyframes animated_div {
    0% {
        left: 0px;
    }
    50% {
        left: 300px;
        background-color: yellow;
        transform: rotate(180deg);
    }
    100% {
        left: 0px;
    }
  }

<!-- index.html: -->
  ...
  <body>
    <h1>Animation</h1>
    <div id="animated_div"></div>
  </body>
  ...  
```

## Reszponzivitás, reszponzív tartalom
- Minden eszközre (mobiltelefon, tablet, pc) ugyanazt a tartalmat küldi a szerver
- A reszponzivitás azt jelenti, hogy CSS segítségével megadhatjuk, hogy az adott eszköz kijelzőjének szélességéhez igazodjon a tartalom
- media query: a böngésző lekér	dezi a megjelenítő médiát és azt, hogy normál (screen) vagy nyomtatási (print) nézetben vagyunk-e
- a @media CSS parancsszóval adhatjuk meg a kijelzőhöz (screen) vagy a nyomtatási nézethez (print) igazodó tartalombeállításokat (pl. nyomtatáskor így elkerülhető a menü kinyomtatása a menüosztálynak display:none tulajdonságot adva)
  pl.: @media only screen and (min-width: 600px) ...
- Ha több @media beállítás is igaz és az ugyanarra az elemre vonatkozó értékek különbözőek, az elem aktuálisan lehetséges legnagyobb kijelzőre vonatkozó beállítási szabálya lesz érvényes
