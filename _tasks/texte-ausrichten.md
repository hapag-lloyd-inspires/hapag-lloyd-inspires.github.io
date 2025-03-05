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
.center {
    text-align: center;
}
</style>

<p>Dieser Text ist links ausgerichtet.</p>
<p class="center">Dieser Text ist zentriert.</p>
</div>

`style.css`
```css
.center {
    text-align: center;
}
```

`index.html`
```html
<p>Dieser Text ist links ausgerichtet.</p>
<p class="center">Dieser Text ist zentriert.</p>
```

{: .task }
> 1. Füge deiner `style.css` Datei eine Klasse hinzu, welcher den Text zentriert. Füge diese Klasse einem Absatz in deinem Projekt hinzu.
> 2. Erstelle eine Klasse, die den Text rechts ausrichtet und füge die Klasse einem weiteren Absatz in deinem Projekt hinzu.
> 3. Experimentiere mit der Ausrichtung des Textes und finde heraus, welche Ausrichtung am besten zu deinem Design passt.