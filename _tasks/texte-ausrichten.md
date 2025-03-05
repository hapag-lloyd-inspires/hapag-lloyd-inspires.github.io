---
layout: post
title:  Texte ausrichten
nav_order: 8
---

# Texte ausrichten

Texte können auf verschiedene Weisen ausgerichtet werden. Die Ausrichtung eines Textes kann das Erscheinungsbild einer Webseite stark beeinflussen. Es gibt drei Hauptausrichtungen für Texte:
- Links ausgerichtet
- Zentriert
- Rechts ausgerichtet

Die Ausrichtung eines Textes kann mit dem `text-align` Attribut geändert werden. Das Attribut nimmt einen der folgenden Werte an:
- `text-align: left;`: Der Text wird linksbündig ausgerichtet.
- `text-align: center;`: Der Text wird zentriert ausgerichtet.
- `text-align: right;`: Der Text wird rechtsbündig ausgerichtet.

<div class="code-example">
<style>
.left {
    text-align: left;
}
.center {
    text-align: center;
}
.right {
    text-align: right;
}
</style>

<p class="left">Dieser Text ist links ausgerichtet.</p>
<p class="center">Dieser Text ist zentriert.</p>
<p class="right">Dieser Text ist rechts ausgerichtet.</p>
</div>

`style.css`
```css
.left {
    text-align: left;
}
.center {
    text-align: center;
}
.right {
    text-align: right;
}
```

`index.html`
```html
<p class="left">Dieser Text ist links ausgerichtet.</p>
<p class="center">Dieser Text ist zentriert.</p>
<p class="right">Dieser Text ist rechts ausgerichtet.</p>
```

{: .task }
> 1. Füge deiner `style.css` Datei die Klassen `.left`, `.center` und `.right` hinzu.
> 2. Ändere die Ausrichtung des Textes in deinem Projekt mit den Klassen `.left`, `.center` und `.right`.
> 3. Experimentiere mit der Ausrichtung des Textes und finde heraus, welche Ausrichtung am besten zu deinem Design passt.