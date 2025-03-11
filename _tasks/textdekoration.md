---
layout: post
title:  Textdekoration
nav_order: 3
---

# Textdekoration

## Das span-Element

Jedes html-Element kann mit dem `style`-Attribut formatiert werden. Das `style`-Attribut enthält CSS-Regeln, die auf das Element angewendet werden.

Versuchen wir mal einen Absatz fett zu drucken.

<div class="code-example py-3">
<p style="font-weight: bold;">Das ist ein fett gedruckter Absatz.</p>
<p>Das ist ein normaler Absatz</p>
</div>
```html
<p style="font-weight: bold;">Das ist ein fett gedruckter Absatz.</p>
<p>Das ist ein normaler Absatz</p>
```

{: .task }
Erstelle einen Absatz, der fett gedruckt ist.

Das funktioniert, aber es ist nicht die beste Methode, um Text zu formatieren. Was, wenn wir nur ausgewählte Wörter fett drucken wollen? Dafür können wir das `<span>`-Element verwenden. Für sich genommen macht das `<span>`-Element keinen visuellen Unterschied:

<div class="code-example py-3">

<p>Das ist ein <span>normaler</span> Text.</p>

</div>
```html
<p>Das ist ein <span>normaler</span> Text.</p>
```

Wenn wir nun das `<span>`-Element mit dem `style`-Attribut verwenden, können wir den Text innerhalb des `<span>`-Elements formatieren.

<div class="code-example py-3">

<p>Das ist ein <span style="font-weight: bold">fetter</span> Text.</p>

</div>
```html
<p>Das ist ein <span style="font-weight: bold">fetter</span> Text.</p>
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
Markiere mindestens drei Wörter in auf deiner Webseite kursiv.

## Letter Spacing

Der Abstand zwischen den Buchstaben eines Textes kann mit dem `letter-spacing`-Attribut geändert werden. Der Wert des `letter-spacing`-Attributs gibt den Abstand zwischen den Buchstaben in Pixeln an. Die Abkürzung `px` steht für Pixel.

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
Markiere mindestens drei Wörter auf deiner Webseite fett und kursiv.
Markiere mindestens ein Wort auf deiner Webseite fett, kursiv und mit größerem Abstand zwischen den Buchstaben.

{: .extra-task }
Finde heraus, wie man einen Text mit der `text-decoration` Regel Wörter <span style="text-decoration: line-through;">durchstreichen</span> und <span style="text-decoration: underline;">unterstreichen</span> kann. Suche dafür in der [Css Referenz](https://www.w3schools.com/cssref/index.php) nach der passenden CSS-Regel.

{: .extra-task }
Erstelle ein `<span>`-Element, das einen Text fett, kursiv, unterstrichen und durchgestrichen darstellt.