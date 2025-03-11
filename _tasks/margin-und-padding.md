---
layout: post
title:  Margin und Padding
nav_order: 10
---
<style>
.hintergrund-rot {
    background-color: red;
}

.meine-box-1 {
    background-color: lightblue;
    width: 200px;
}

.meine-box-mit-padding {
    background-color: lightblue;
    width: 200px;
    padding-top: 20px;
    padding-bottom: 40px;
    padding-left: 10px;
}

.box-1 {
    background-color: rgb(30,195,255);
    width: 200px;
    padding: 10px;
}

.box-2 {
    background-color: rgb(255,30,30);
    width: 300px;
    padding: 10px;
}

.box-mit-border {
    background-color: rgb(255, 255, 255);
    border-color: rgb(44, 132, 250);
    border-width: 1px;
    border-style: solid;
    width: 200px;
    padding: 10px;
    margin-bottom: 20px;
}

.margin-bottom-10 {
    margin-bottom: 10px;
}

.margin-left-50 {
    margin-left: 50px;
}

.hintergrund-orange {
    background-color: orange;
}

.hintergrund-rot {
    background-color: red;
}

.text-weiss {
    color: white;
}

.padding-50 {
    padding: 50px;
}

.margin-obenunten-20 {
    margin-top: 20px;
    margin-bottom: 20px;
}

.comic {
    font-family: 'Comic Sans MS', cursive;
}

.padding-links-100 {
    padding-left: 100px;
}

</style>

# Margin und Padding

## Das Div-Element

Das `<div>`-Element ist ein Container-Element, das verwendet wird, um andere Elemente zu gruppieren und zu strukturieren. Es hat keine spezifische Bedeutung, sondern dient dazu, den Inhalt der Webseite in Abschnitte zu unterteilen und zu organisieren. Es ist ähnlich wie das `<span>`-Element, aber es wird normalerweise für größere Abschnitte von Inhalten verwendet.


Ein Beispiel:

<div class="code-example">
<div>ein Div</div>
</div>

```html
<div>ein Div</div>
```

Wie du siehst, macht das `<div>`-Element keinen visuellen Unterschied. Es ist nur ein Container, der verwendet wird, um andere Elemente zu gruppieren.

Wir können dem div auch eine Klasse hinzufügen:

<div class="code-example">
<div style="background-color: cornflowerblue">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
}
```

`index.html`
```html
<div class="box">ein Div</div>
```

Und eine Breite:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
}
```

## Padding

Außerdem können wir dem div auch padding hinzufügen. Padding ist der Abstand zwischen dem Inhalt des Elements und seinem Rand:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding: 30px;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    padding: 30px;
}
```

Wie du siehst bedeutet `padding: 30px;`, dass der Abstand zwischen dem Inhalt des Elements und allen 4 Rändern 30 Pixel beträgt.



## Margin

Lass uns auch noch den Margin hinzufügen. Margin ist der Abstand zwischen den Rändern von zwei Elementen:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding: 30px; margin: 50px">ein Div</div>

</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    padding: 30px;
    margin: 50px;
}
```



{: .task }
> 1. Erstelle ein `<div>` Element und füge dem Element eine Klasse hinzu.
> 2. Füge die Klasse in deiner `style.css` Datei hinzu. Denk daran den `.` vor dem Klassennamen zu setzen.
> 3. Ändere folgendes an deinem `<div>` Element mit der Klasse:
>    1. Hintergrundfarbe
>    2. Breite
>    3. Padding
>    4. Margin
> 4. Füge ein weiteres `<div>` Element hinzu und füge ihm eine andere Klasse hinzu. Wiederhole die Schritte 2 und 3.

## Padding auf einer Seite

Wir können auch nur das Padding auf einer Seite anwenden:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding-top: 30px;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    padding-top: 30px;
}
```

## Margin auf einer Seite

Wir können auch nur den Margin auf einer Seite anwenden:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding: 30px; margin-top: 50px">ein Div</div>
</div>

`style.css`
```css

.box {
    background-color: cornflowerblue;
    width: 200px;
    padding: 30px;
    margin-top: 50px;
}
```

{: .task }
> Experimentiere mit dem Padding und Margin auf einer Seite. 

## Kurze Schreibweise für Padding und Margin

Es gibt auch eine Kurzschreibweise für Padding und Margin:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; margin: 1px 50px;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    margin: 10px 50px;
}
```

Was bedeutet das? Die erste Zahl ist der Abstand oben und unten, die zweite Zahl ist der Abstand links und rechts. Das bedeutet `margin: 30px 50px;` ist das gleiche wie `margin-top: 30px; margin-bottom: 30px; margin-left: 50px; margin-right: 50px;`.

Wenn wir zum Beispiel nur den Margin oder das Padding links und rechts ändern wollen, können wir das so machen:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding: 0 30px; margin: 0 50px;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    padding: 0 30px;
    margin: 0 50px;
}
```

{: .task }
> Experimentiere mit der Kurzschreibweise für Padding und Margin.

## Divs Zentrieren


Wir können auch divs zentrieren:

<div class="code-example">
<div style="background-color: cornflowerblue; width: 200px; padding: 30px; margin: 0 auto;">ein Div</div>
</div>

`style.css`
```css
.box {
    background-color: cornflowerblue;
    width: 200px;
    padding: 30px;
    margin: 0 auto;
}
```

{: .task }
> Wenn es zu deinem Design passt, zentriere einige deiner divs.


## Beispiele mit Margin und Padding

Margin und Padding sind zwei wichtige Konzepte in CSS, um mächtige Design umzusetzen. Zum Beipsiel kannst du folgendes machen:

<div class="code-example">
<div class="hintergrund-orange text-weiss padding-50 margin-obenunten-20">
<h1>Willkommen!</h1>
<p>Das ist ein Abschnitt auf deiner Webseite</p>
</div>
<div class="hintergrund-rot text-weiss padding-50 padding-links-100 margin-obenunten-20">
<h1>Über uns</h1>
<p>Das ist ein weiterer Abschnitt</p>
</div>
</div>

```css
.hintergrund-orange {
    background-color: orange;
}

.hintergrund-rot {
    background-color: red;
}

.text-weiss {
    color: white;
}

.padding-50 {
    padding: 50px;
}

.padding-links-100 {
    padding-left: 100px;
}

.margin-obenunten-20 {
    margin-top: 20px;
    margin-bottom: 20px;
}
```

```html
<div class="hintergrund-orange text-weiss padding-50 margin-obenunten-20">
    <h1>Willkommen!</h1>
    <p>Das ist ein Abschnitt auf deiner Webseite</p>
</div>
<div class="hintergrund-rot text-weiss padding-50 margin-obenunten-20 padding-links-100">
    <h1>Über uns</h1>
    <p>Das ist ein weiterer Abschnitt</p>
</div>
```


## Elemente mittig ausrichten

Wenn du ein `div` Element hast, kannst du es mittig ausrichten, indem du `margin: 0 auto;` in der `style.css` Datei hinzufügst.

<div class="code-example py-7">
<style>
.container {
    width: 50%;
    border: 1px solid #000;
    padding: 10px;
    margin-bottom: 10px;
}
.center-container {
    margin: 0 auto;
}
</style>
<div class="container">
    <p>Ich bin in einem Container.</p>
    <p>Ich bin in einem Container.</p>
</div>
<div class="container center-container">
    <p>Ich bin in einem Container.</p>
    <p>Ich bin in einem Container.</p>
</div>
</div>
`index.html`
```html
<div class="container">
    <p>Ich bin in einem Container.</p>
    <p>Ich bin in einem Container.</p>
</div>
<div class="container center-container">
    <p>Ich bin in einem Container.</p>
    <p>Ich bin in einem Container.</p>
</div>
```
`style.css`
```css
.container {
    width: 50%;
    margin: 0 auto;
    border: 1px solid #000;
    padding: 10px;
    margin-bottom: 10px;
}
.center-container {
    margin: 0 auto;
}
```

{: .task }
Erstelle einen Container und richte ihn mittig aus.

{: .task }
Experimentiere heraus, wie du das neu gelernte am Besten in deinem Projekt verwenden kannst.