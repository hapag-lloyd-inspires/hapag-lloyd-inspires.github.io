---
layout: post
title:  Schriftarten
nav_order: 7
---

# Schriftarten

Schriftarten sind ein wichtiger Bestandteil des Designs einer Webseite. Sie können die Lesbarkeit und das Erscheinungsbild einer Webseite stark beeinflussen. Es gibt viele verschiedene Schriftarten, die für Webseiten verwendet werden können. Einige der beliebtesten Schriftarten sind:
- <span style="font-family: Arial">Arial</span>
- <span style="font-family: Franklin Gothic Medium">Franklin Gothic Medium</span>
- <span style="font-family: 'Courier New', Courier, monospace;">Courier New</span>
- <span style="font-family: 'Verdanta;">Verdanta</span>
- <span style="font-family: 'Times New Roman', Times, serif;">Times New Roman</span>
- <span style="font-family: 'Comic Sans MS', cursive;">Comic Sans MS</span>
- <span style="font-family: 'Lucida Console', Monaco, monospace;">Lucida Console</span>
- <span style="font-family: 'Trebuchet MS', Helvetica, sans-serif;">Trebuchet MS</span>
- <span style="font-family: 'Georgia', serif;">Georgia</span>
- <span style="font-family: 'Palatino Linotype', 'Book Antiqua', Palatino, serif;">Palatino Linotype</span>
- <span style="font-family: 'Arial Black', Gadget, sans-serif;">Arial Black</span>
- <span style="font-family: 'Impact', Charcoal, sans-serif;">Impact</span>
- <span style="font-family: 'Tahoma', Geneva, sans-serif;">Tahoma</span>
- <span style="font-family: 'Consolas">Consolas</span>



## Schriftart ändern

Die Schriftart einer Webseite kann mit dem `font-family` Attribut geändert werden. Das Attribut nimmt eine Liste von Schriftarten an, die in der Reihenfolge angegeben werden, in der sie verwendet werden sollen. Wenn die erste Schriftart nicht verfügbar ist, wird die nächste Schriftart in der Liste verwendet.

<div class="code-example">
<style>
.arial {
    font-family: Arial, sans-serif;
}
.comic-sans {
    font-family: 'Comic Sans MS', cursive;
}
</style>
<p class="arial">Dieser Text ist in der Schriftart Arial.</p>
<p class="comic-sans">Dieser Text ist in der Schriftart Comic Sans MS.</p>
<p style="font-family: 'Courier New', Courier, monospace;">Dieser Text ist in der Schriftart Courier New.</p>
</div>
`style.css`
```css
.arial {
    font-family: Arial, sans-serif;
}
.comic-sans {
    font-family: 'Comic Sans MS', cursive;
}
```
`index.html`
```html
<p class="arial">Dieser Text ist in der Schriftart Arial.</p>
<p class="comic-sans">Dieser Text ist in der Schriftart Comic Sans MS.</p>
<p style="font-family: 'Courier New', Courier, monospace;">Dieser Text ist in der Schriftart Courier New.</p>
```

{: .task }
> 1. Ändere die Schriftart des Textes in deinem Projekt mit dem style-Attribut `font-family`.
> 2. Ändere die Schriftart eines Absatzes in deinem Text mit einer Klasse in der `style.css` Datei.
> 3. Probiere verschiedene Schriftarten aus und wähle diejenige aus, die dir am besten gefällt.