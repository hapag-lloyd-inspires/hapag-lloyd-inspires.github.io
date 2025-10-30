---
layout: post
title:  Aufgaben
nav_order: 1
---
# Aufgaben

## Unsere Mission
Erstelle einen Steckbrief als Webseite zu einem Thema deiner Wahl. Verwende das in der Hackerschool gelernte Wissen, um die Webseite zu stylen. Am Ende der Hackerschool wirst du deine Webseite vorstellen.

Beispiele:
- [Igel](https://hapag-lloyd-inspires.github.io/examples/HLHackerSchool25Dekarz/)
- [3D Druck](https://hapag-lloyd-inspires.github.io/examples/Beispiel%20Steckbrief%203D-Druck/)
- [Hapag-Lloyd](https://hapag-lloyd-inspires.github.io/examples/hapag-lloyd-1/)

## Teil 1: Grundlagen

1. Wähle ein Thema, zu dem du eine Webseite erstellen möchtest.
2. Erstelle mindestens 3 Überschriften und mindestens 3 Absätze. Verwende dazu die Elemente `h1`, `h2`, `h3` und `p`.
3. Hebe wichtige Wörter mit den html-Elementen `em`, `strong` und `u` hervor.
4. Erstelle eine Liste. Verwende dazu die Elemente `ul` und `li`.
5. Füge eine horizontale Linie mit dem `hr` Element hinzu.
Zusatz:
6. Markiere wichtigen Text auf deiner Webseite. Lese dazu [diesen Artikel](https://developer.mozilla.org/de/docs/Web/HTML/Reference/Elements/mark).
7. Erstelle eine Tabelle. Lies dazu [diesen Artikel](https://www.w3schools.com/html/html_tables.asp).

## Teil 2: Attribute, Bilder und Farben
1. Füge deiner Webseite mindestens 3 Links hinzu. Verwende dazu das html Element `<a href="...">...</a>`
2. Füge mindestens 3 Bilder hinzu. Nutze dazu `<img src="..." alt=".." width="..." />`
3. Ändere die Schriftfarbe und die Hintergrundfarbe von mindestens 5 Elementen. Verwende den [Color-Picker](https://www.w3schools.com/colors/colors_picker.asp) um Farben zu finden.
Zusatz
3. Verwende das Element `abbr` und das Attribut `title` für eine Abkürzung in deinem Text. Lies [dieses Tutorial](https://www.w3schools.com/html/html_quotation_elements.asp) für mehr Informationen.
4. Finde heraus, wie man im `style` Attribut einen Absatz oder eine Überschrift zentriert. Schau dir [hier](https://www.w3schools.com/css/css_text_align.asp) die `text-align` Eigenschaft an.
5. Finde heraus, wie man einen Rahmen um einen Absatz oder eine Überschrift setzt. Erstelle mindestens 3 Rahmen mit unterschiedlicher Stärke, Farbe und Style. [Hier](https://www.w3schools.com/css/css_border.asp) findest du eine Anleitung dazu.

## Teil 3: Css 
1. Erstelle ein html, head, style und body Element für deine Seite

```html
<html>
<head>
<style>
  /* deine css Anweisungen */
</style>
</head>
<body>
  <!-- Dein bisheriger Quelltext -->
</body>
</html
```
2. Ändere die Hintergrundfarbe der gesamten Webseite.

```html
<style>
body {
    background-color: rgb(194, 214, 214);
}
</style>
```

2. Ändere die Farbe und Schriftgröße aller Absätze und Überschriften.

```html
<style>
p {
  color: rgb(0, 0, 0);
  background-color: rgb(0, 0, 0);
  font-size: 12px;
}
h1 {
    ...
}
h2 {
    ...
}    
</style>
```

3. Ändere die Schriftart aller Absätze sowie aller h1, h2 und h3 überschriften. [Hier](https://www.w3schools.com/css/css_font.asp) findest du mögliche Schriftarten. 

```html
p {
   ...
   font-family: "Lucida Console";
}

h1 {
  ...
  font-family: ...;
}
h2 { ... }
h3 { ... }
```

4. Ändere die Farbe und Schriftart aller deiner Links. Tipp: Nutze die Form `a { ... }` im css-Teil deiner Webseite.
5. Verwende die css-Eigenschaft für deine Überschriften und Absätze. Die Verwendung findest du [hier](https://developer.mozilla.org/de/docs/Web/CSS/text-align).

## Border, padding und marging
1. Füge deinen Bildern einen Rahmen hinzu.

## Schon fertig mit den Aufgaben?
- Füge Emoji's auf deine Webseite ein. [Hier](https://www.w3schools.com/html/html_emojis.asp) findest du ein Tutorial.
- Füge ein YouTube Video über auf deiner Seite ein. [Hier](https://www.w3schools.com/html/html_youtube.asp) sind mehr Informationen darüber.
- Lerne, wie man das [Canvas](https://www.w3schools.com/html/html5_canvas.asp) Element benutzt und erarbeite einen 5-Minuten Vortrag mit einem Beispiel. [Hier](https://www.w3schools.com/tags/ref_canvas.asp) sind noch mehr Beispiele.