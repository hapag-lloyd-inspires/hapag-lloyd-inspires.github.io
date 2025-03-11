---
layout: post
title:  Farbe
nav_order: 5
---
# Farben

## Textfarbe

Die Farbe des Textes kann mit dem `color`-Attribut geändert werden.

Die Regel `color: red;` bedeutet "Farbe: rot".

<div class="code-example py-3">
<p>Meine Lieblingsfarben sind <span style="color: red;">rot</span>, <span style="color: orange;">orange</span> und <span style="color: green;">grün</span>.</p>
</div>
```html
<p>Meine Lieblingsfarben sind <span style="color: red;">rot</span>, <span style="color: orange;">orange</span> und <span style="color: green;">grün</span>.</p>
```

{: .task }
Färbe drei Wörter in deinem Text in verschiedenen Farben ein.

## Darstellung von Farben

Es gibt verschiedene Möglichkeiten, Farben in CSS zu definieren. Die einfachste Möglichkeit ist, den Namen der Farbe zu verwenden, jedoch stehen so nur 16 Farben zur Verfügung.

Du kannst auch mit der css-Funktion `rgb()` Farben definieren. Die Funktion nimmt drei Werte an, die die Intensität der Farben Rot, Grün und Blau angeben. Jeder Wert kann zwischen 0 und 255 liegen.

Zum Beispiel bedeutet `rgb(255, 0, 0)` "rot" und `rgb(0, 255, 0)` "grün".

<div class="code-example py-3">
<p>
Meine Lieblingsfarben sind <span style="color: rgb(0, 0, 255);">blau</span>, <span style="color: rgb(255, 0, 0);">rot</span> und <span style="color: rgb(0, 255, 0);">grün</span>.
</p></div>
```html
<p>
Meine Lieblingsfarben sind 
<span style="color: rgb(0, 0, 255);">blau</span>, 
<span style="color: rgb(255, 0, 0);">rot</span> und 
<span style="color: rgb(0, 255, 0);">grün</span>.
</p>
```

{: .task }
> - Färbe mindestens 3 Wörter in verschiedenen Farben mit dem englischen Namen der Farbe ein.
> - Färbe mindestens 3 Wörter in verschiedenen Farben mit der rgb() Funktion ein.
> - Färbe mindestens 3 Wörter in verschiedenen Farben mit den RGB-Werten vom [Color Picker](https://www.w3schools.com/colors/colors_picker.asp).

## Hintergrundfarbe

Neben der Textfarbe kann auch die Hintergrundfarbe eines Elements geändert werden. Dazu wird das css `background-color` Attribut verwendet.

<div class="code-example py-3">
 <p>Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins <span style="background-color: rgb(255, 255, 0);">19. Jahrhundert</span> zurück ... </p>
</div>
```html
<p>
    Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins <span style="background-color: rgb(255, 255, 0);">19. Jahrhundert</span> zurück ... 
</p>
```

{: .task }
Markiere mindestens 3 Wörter deines Textes mit einer Hintergrundfarbe, als wären sie mit einem Textmarker markiert.

## Background-color und Textfarbe kombinieren

Es ist auch möglich, die Hintergrundfarbe eines Elements zu ändern und gleichzeitig die Textfarbe zu ändern.

<div class="code-example py-3">
<p>
    der
    <span style="background-color: black; color: white;">Winter</span>
</p>
</div>
```html
<p>
    der
    <span style="background-color: black; color: white;">Winter</span>
</p>
```

{: .task }
Färbe mindestens 3 Wörter in deinem Text so ein, dass die Hintergrundfarbe und die Textfarbe unterschiedlich sind.

## Hintergrundfarbe eines Absatzes ändern

Es ist auch möglich, die Hintergrundfarbe eines ganzen Absatzes zu ändern.

<div class="code-example py-3">
<h2 style="background-color: rgb(65, 214, 147); color: white;">Zitate</h2>
<p style="background-color: rgb(189, 203, 245); font-style: italic;"> 
    “Hab den Mut, deinem Herzen und deiner Intuition zu folgen. Du weißt schon, wer du gerne werden möchtest. Alles andere ist unwichtig.”
</p>
<p style="background-color: #7be2f9;">
    Steve Jobs
</p>
</div>
```html
<h2 style="background-color: rgb(65, 214, 147); color: white;">Zitate</h2>
<p style="background-color: rgb(189, 203, 245); font-style: italic;"> 
    “Hab den Mut, deinem Herzen und deiner Intuition zu folgen. Du weißt schon, wer du gerne werden möchtest. Alles andere ist unwichtig.”
</p>
<p style="background-color: #7be2f9;">
    Steve Jobs
</p>
```
Jetzt haben wir schon mal einiges an Farbe auf unsere Webseite gebracht. In den nächsten Schritten werden wir noch mehr Möglichkeiten kennenlernen, wie wir unsere Webseite noch schöner gestalten können.

{: .task }
Füge deinem Text mindestens einen Absatz hinzu, der eine Hintergrundfarbe hat und eine andere Textfarbe. Kombiniere verschiedene css-Regeln, sodass deine Seite interessanter aussieht.

{: .extra-task }
> Ändere die Farbe jedes Buchstabens einer Überschrift in eine andere Farbe. Zum Beispiel:
> 
> <span style="color: red;">H</span><span style="color: orange;">a</span><span style="color: yellow;">p</span><span style="color: green;">a</span><span style="color: blue;">g</span><span style="color: indigo;">-</span><span style="background-color: violet;">L</span><span style="color: white; background-color: red;">l</span><span style="background-color: orange; color: white">o</span><span style="background-color: yellow;">y</span><span style="background-color: green; color: white">d</span> oder  <span style="background-color: orange; color: white;">H</span><span style="background-color: blue; color: white;">a</span><span style="background-color: orange; color: white;">p</span><span style="background-color: blue; color: white;">a</span><span style="background-color: orange; color: white;">g</span><span style="background-color: blue; color: white;">-</span><span style="background-color: orange; color: white;">L</span><span style="background-color: blue; color: white;">l</span><span style="background-color: orange; color: white;">o</span><span style="background-color: blue; color: white;">y</span><span style="background-color: orange; color: white;">d</span> 
