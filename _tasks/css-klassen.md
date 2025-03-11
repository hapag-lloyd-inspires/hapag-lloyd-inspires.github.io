---
layout: post
title:  CSS Klassen
nav_order: 6
---
# CSS Klassen

In der letzten Aufgabe hast du viele Textabschnitte mit einer Hintergrundfarbe <span style="background-color: orange">markiert.

{: .task }
markiere *jetzt* mindestens 5 wichtige Fakten mit einer gelben Hintergrundfarbe.

<div class="code-example">
<p>
    <span style="background-color: yellow">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span style="background-color: yellow">Datenanalyse</span>, <span style="background-color: yellow">Webentwicklung</span> und <span style="background-color: yellow">künstlichen Intelligenz</span> eingesetzt.
</p>
<p>
    <span style="background-color: yellow">JavaScript</span> hingegen ist die Hauptsprache für die Entwicklung <span style="background-color: yellow">interaktiver Webseiten</span>.
</p>
</div>

```html
<p>
    <span style="background-color: yellow">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span style="background-color: yellow">Datenanalyse</span>, <span style="background-color: yellow">Webentwicklung</span> und <span style="background-color: yellow">künstlichen Intelligenz</span> eingesetzt.
</p>
<p>
    <span style="background-color: yellow">JavaScript</span> hingegen ist die Hauptsprache für die Entwicklung <span style="background-color: yellow">interaktiver Webseiten</span>.
</p>
```

Was ist, wenn du die Hintergrundfarbe ändern möchtest, zum Beispiel von gelb zu blau?

{: .task }
Ändere die Hintergrundfarbe aller markierten Wörter in deinem Projekt zu <span style="background-color: lightblue">hellblau</span>.

Was hast du getan? Du musstest jedes `<span>` Element einzeln ändern. Das ist mühsam und zeitaufwändig. Es gibt eine bessere Lösung: CSS Klassen.

## CSS Klassen

CSS Klassen sind eine Möglichkeit, um mehrere Elemente mit dem gleichen Stil zu versehen. Eine Klasse ist ein Name, der in einem HTML-Element verwendet wird, um es mit einem bestimmten Stil zu versehen.

Ein Beispiel:

<div class="code-example">
<style>
.marker {
    background-color: lightblue;
}
</style>
<p>
    <span  class="marker">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span  class="marker">Datenanalyse</span>, <span  class="marker">Webentwicklung</span> und <span  class="marker">künstlichen Intelligenz</span> eingesetzt.
</p>
<p>
    <span  class="marker">JavaScript</span> hingegen ist die Hauptsprache für die Entwicklung <span  class="marker">interaktiver Webseiten</span>.
</p>
</div>
`style.css`
```css
.marker {
    background-color: lightblue;
}
```
`index.html`
```html
<p>
    <span  class="marker">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span  class="marker">Datenanalyse</span>, <span  class="marker">Webentwicklung</span> und <span  class="marker">künstlichen Intelligenz</span> eingesetzt.
</p>
<p>
    <span  class="marker">JavaScript</span> hingegen ist die Hauptsprache für die Entwicklung <span  class="marker">interaktiver Webseiten</span>.
</p>
```


In diesem Beispiel haben wir eine Klasse `marker` erstellt, die den Hintergrund der Elemente auf `lightblue` setzt. Diese Klasse wird dann in den `<span>` Elementen in dem `class=` Attribut verwendet, um sie mit dem Stil zu versehen.

Wir können jetzt einfach über die Klasse `marker` in der `style.css` Datei den Stil aller markierten Wörter ändern. Die `index.html` Datei bleibt unberührt. Zum Beispiel:

<div class="code-example">
<style>
.marker-2 {
    background-color: greenyellow;
}
</style>
<p>
    <span  class="marker-2">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span  class="marker-2">Datenanalyse</span>, <span  class="marker-2">Webentwicklung</span> und <span  class="marker-2">künstlichen Intelligenz</span> eingesetzt.
</p>
</div>
`style.css`
```css
.marker {
    background-color: greenyellow;
}
```


Füge Klassen in deiner `style.css` Datei hinzu. **Wichtig**: Klassen in css beginnen mit einem Punkt `.`. In html werden sie ohne Punkt verwendet.

{: .task }
> 1. Erstelle eine Klasse in deiner `style.css` Datei, die den Hintergrund der Elemente auf `lightblue` setzt. Nenne sie zum Beispiel `marker` oder `highlight`.
> 2. Verwende diese Klasse in deinem Projekt, um die Hintergrundfarbe aller markierten Wörter zu ändern.
> 3. Überprüfe, ob die Hintergrundfarbe aller markierten Wörter geändert wurde.
> 4. Ändere die Hintergrundfarbe der Klasse in deiner `style.css` Datei zu einer anderen Farbe und überprüfe, ob die Hintergrundfarbe aller markierten Wörter geändert wurde.

{: .task }
> 1. Erstelle eine Klasse in deiner `style.css` Datei, die den Text in den Elementen fett macht. Nenne sie zum Beispiel `fetter-text`.
> 2. Verwende diese Klasse in deinem Projekt, um den Text in den markierten Wörtern fett zu machen.

{: .task }
Was passiert, wenn du die Klasse `.marker { ... } ` ohne den Punkt (`marker { ... }`) in deiner `style.css` Datei erstellst? 

## Css Anweisungen kombinieren

Du kannst auch mehrere CSS Anweisungen in einer Klasse kombinieren. Zum Beispiel:

<div class="code-example">
<style>
.marker-3 {
    background-color: greenyellow;
    font-weight: bold;
    letter-spacing: 2px;
}
</style>
<p>
    <span  class="marker-3">Python</span> ist besonders bekannt für seine einfache Syntax und wird häufig in der <span  class="marker-3">Datenanalyse</span>, <span  class="marker-3">Webentwicklung</span> und <span  class="marker-3">künstlichen Intelligenz</span> eingesetzt.
</p>
</div>
`style.css`
```css
.marker {
    background-color: greenyellow;
    font-weight: bold;
    letter-spacing: 2px;
}
```

{: .task }
Probiere selbst aus, wie du verschiedene CSS Anweisungen in einer Klasse kombinieren kannst. Erstelle drei Klassen, die den Text unterschiedlich gestalten. Verwende diese Klassen in deinem Projekt.

## Klassen kombinieren

Du kannst auch mehrere Klassen in einem Element verwenden. Wenn du mehrere Klassen in einem Element verwendest, werden die Stile der Klassen kombiniert.

<div class="code-example">
<style>
.marker-gruen {
    background-color: rgb(39, 221, 39);
}
.marker-orange {
    background-color: rgb(255, 165, 0);
}
.fetter-text {
font-weight: bold;
}
</style>
<p>
    Dieser Text ist <span class="marker-gruen fetter-text">hervorgehoben und fett.</span>
</p>
<p>
    <span class="fetter-text">Folgender</span> Text ist <span class="marker-orange">orange.</span>
</p>
</div>

`style.css`

```css
.marker-gruen {
    background-color: rgb(39, 221, 39);
}

.marker-orange {
    background-color: rgb(255, 165, 0);
}

.fetter-text {
    font-weight: bold;
}
```
`index.html`
```html
<p>
    <span class="marker-gruen fetter-text">Dieser Text ist hervorgehoben und fett.</span>
    <span class="marker-orange">Dieser Text ist orange.</span>
</p>
```

{: .task }
> 1. Erstelle zwei Klassen `kursiver-text` und eine Klasse `fetter-text` in deiner `style.css` Datei. Mache anschließend einige Wörte in deinem Projekt kursiv und fett.
> 2. Erstelle eine Klasse `weisser-text` in deiner `style.css` Datei, die den Text weiß färbt. Verwende diese Klasse in deinem Projekt, um den Text weiß zu färben.
> 3. Kombiniere eine Klasse `weisser-text` mit einer anderen Klasse die den Hintergrund z.B. schwarz färbt.

<div class="code-example">
Sherlock <span style="background-color: black; color: white;">Holmes</span>
