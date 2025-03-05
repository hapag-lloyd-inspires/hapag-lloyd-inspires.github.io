---
layout: post
title:  Textdekoration
nav_order: 4
---

# Textdekoration

## Das span-Element

Jedes html-Element kann mit dem `style`-Attribut formatiert werden. Das `style`-Attribut enthält CSS-Regeln, die auf das Element angewendet werden.

Das `<span>`-Element ist ein Inline-Element, das dazu verwendet wird, um Teile eines Textes zu formatieren. Für sich genommen macht das `<span>`-Element keinen visuellen Unterschied:

<div class="code-example py-3">

<p>Das ist ein <span>normaler</span> Text.</p>

</div>
```html
<p>Das ist ein <span>normaler</span> Text.</p>
```


Das `<span>`-Element wird oft verwendet, um Textfarbe, Schriftgröße oder Schriftart zu ändern.

<div class="code-example py-3">
<p>Das ist ein <span style="font-weight: bold;">fetter</span> Text.</p>
</div>
```html
<p>Das ist ein <span style="font-weight: bold;">fetter</span> Text.</p>
```

Die Anweisungen, welche im style-Attribut stehen, sind CSS-Regeln. `font-weight: bold;` heißt auf Deutsch "Schriftgewicht: fett".

{: .task }
Erstelle 4 `<span>`-Elemente, die einen Text fett darstellt.

## Kursivschrift

Kursivschrift wird oft verwendet, um Zitate oder Buchtitel hervorzuheben. Das `font-style`-Attribut wird verwendet, um Text kursiv zu machen.

Die Regel `font-style: italic;` bedeutet "Schriftstil: kursiv".

<div class="code-example py-3">
<p>Das Buch <span style="font-style: italic;">Harry Potter</span> ist sehr beliebt.</p>
</div>
```html
<p>Das Buch <span style="font-style: italic;">Harry Potter</span> ist sehr beliebt.</p>
```



{: .task }
Erstelle ein `<span>`-Element, das einen Text kursiv darstellt.

## Letter Spacing

Der Abstand zwischen den Buchstaben eines Textes kann mit dem `letter-spacing`-Attribut geändert werden.

<div class="code-example py-3">
<p><span style="letter-spacing: 15px;">Python</span> ist eine beliebte <span style="letter-spacing: 5px;">Programmiersprache</span></p>
</div>
```html
<p>
  <span style="letter-spacing: 15px;">Python</span> ist eine beliebte <span style="letter-spacing: 5px;">Programmiersprache</span>
</p>
```

{: .task }
Erstelle ein `<span>`-Element, das den Abstand zwischen den Buchstaben eines Textes vergrößert.

## Kombination von Textdekorationen

Text kann auf verschiedene Weisen dekoriert werden. Zum Beispiel kann Text fett und kursiv dargestellt sein. Dazu können die CSS-Regeln kombiniert werden und mit Semi-Colons (`;`) getrennt werden. Das sieht dann zum Beispiel so aus:

<div class="code-example py-3">
<p>Das ist <span style="font-style: italic; font-weight: bold;">cooler</span> Text.</p>
</div>
```html
<p>Das ist <span style="font-style: italic; font-weight: bold;">cooler</span> Text.</p>
```

{: .task }
Erstelle ein `<span>`-Element, das einen Text fett und kursiv darstellt.

{: .extra-task }
Finde heraus, wie man einen Text mit der `text-decoration` Regel <span style="text-decoration: line-through;">durchstreichen</span> und <span style="text-decoration: underline;">unterstreichen</span> kann. Suche dafür in der [Css Referenz](https://www.w3schools.com/cssref/index.php) nach der passenden CSS-Regel.

{: .extra-task }
Erstelle ein `<span>`-Element, das einen Text fett, kursiv, unterstrichen und durchgestrichen darstellt.