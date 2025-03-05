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
<div>
    <h1>Überschrift</h1>
    <p>Ein Absatz mit Text.</p>
</div>
</div>

```html
<div>
    <h1>Überschrift</h1>
    <p>Ein Absatz mit Text.</p>
</div>
```

Wie du siehst macht das `<div>`-Element keinen visuellen Unterschied. 

Aber: was ist, wenn wir sowohl die Überschrift als auch den Absatz mit einer anderen Hintergrundfarbe haben möchten?

Probieren wir aus, was passiert, wenn wir die Hintergrundfarbe des `<h1>`-Elements und des `<p>`-Elements ändern:

<div class="code-example">
<div>
    <h1 class="hintergrund-rot">Überschrift</h1>
    <p class="hintergrund-rot">Ein Absatz mit Text.</p>
</div>
</div>

```html
<div>
    <h1 class="hintergrund-rot">Überschrift</h1>
    <p class="hintergrund-rot">Ein Absatz mit Text.</p>
</div>
```

Hmm, das hat nicht funktioniert. Die Hintergrundfarbe wurde nur auf den Text angewendet, nicht auf den gesamten Abschnitt.

<div class="code-example">
<div class="hintergrund-rot">
    <h1>Überschrift</h1>
    <p>Ein Absatz mit Text.</p>
</div>
</div>

```html
<div class="hintergrund-rot">
    <h1>Überschrift</h1>
    <p>Ein Absatz mit Text.</p>
</div>
```

## Breite von Divs

Ähnlich wie Bilder können divs auch eine Breite haben:

<div class="code-example">
<div class="meine-box-1" style="width: 200px;">
<p>Meine Box</p>
</div>
</div>

`style.css`
```css
.meine-box {
    background-color: lightblue;
    width: 200px;
}
```

```html
<div class="meine-box">
<p>Meine Box</p>
</div>
```

{: .task }
Erstelle eine Box wie oben. Ändere die Breite der Box und beobachte, was passiert.

## Padding

Padding ist der Abstand zwischen dem Inhalt eines Elements und seinem Rand. Es wird verwendet, um den Inhalt eines Elements von seinem Rand zu trennen und ihm mehr Platz zu geben.

Das Padding kann mit CSS definiert werden. Die Werte können in Pixeln oder Prozent angegeben werden.

Ein Beispiel:

<div class="code-example">
<div class="meine-box-mit-padding">
<p>Meine Box</p>
</div>
</div>

```css
.meine-box {
    background-color: lightblue;
    width: 200px;
    padding-top: 20px;
    padding-bottom: 40px;
    padding-left: 10px;
}
```

```html
<div class="meine-box">
<p>Meine Box</p>
</div>
```

{: .task }
Erstelle eine Box wie oben. Ändere das Padding der Box und beobachte, was passiert.

## Margin

Margin ist der Abstand zwischen den Rändern von zwei Elementen. Es wird verwendet, um den Abstand zwischen den Elementen zu steuern und ihnen mehr Platz zu geben.

Beispiel:

<div class="code-example">
<div class="box box-1">
<p>Box 1</p>
</div>
<div class="box box-2">
<p>Box 2</p>
</div>
</div>

```css
.box-1 {
    background-color: blue;
    width: 200px;
    padding: 10px;
}

.box-2 {
    background-color: red;
    width: 300px;
    padding: 10px;
}
```

```html
<div class="box-1">
    <p>Box 1</p>
</div>
<div class="box-2">
    <p>Box 2</p>
</div>
```

Die Boxen haben keinen Abstand zwischen ihnen. Was passiert, wenn wir Margin hinzufügen?

<div class="code-example">
<div class="box box-1 margin-bottom-10">
<p>Box 1</p>
</div>
<div class="box box-2">
<p>Box 2</p>
</div>
</div>

```css
.box-1 {
    background-color: blue;
    width: 200px;
    padding: 10px;
}

.box-2 {
    background-color: red;
    width: 300px;
    padding: 10px;
}
.margin-bottom-10 {
    margin-bottom: 10px;
}
```

```html
<div class="box-1 margin-bottom-10">
    <p>Box 1</p>
</div>
<div class="box-2">
    <p>Box 2</p>
</div>
```

Wir können auch Margin auf anderen Seiten anwenden, zum Beispiel Links:

<div class="code-example">
<div class="box box-1 margin-bottom-10 margin-left-50">
<p>Box 1</p>
</div>
<div class="box box-2">
<p>Box 2</p>
</div>
</div>

```css
.box-1 {
    background-color: blue;
    width: 200px;
    padding: 10px;
}

.box-2 {
    background-color: red;
    width: 300px;
    padding: 10px;
}
.margin-bottom-10 {
    margin-bottom: 10px;
}
.margin-left-50 {
    margin-left: 50px;
}
```

```html
<div class="box-1 margin-bottom-10 margin-left-50">
    <p>Box 1</p>
</div>
<div class="box-2">
    <p>Box 2</p>
</div>
```

{: .task }
> 1. Erstelle zwei Boxen wie oben. Experimentiere mit dem Margin und finde heraus, wie es das Layout beeinflusst.
> 2. Füge einer der Boxen einen Rahmen hinzu. Experimentiere mit dem Padding und finde heraus, wie es das Layout beeinflusst.

## Anwendung von Margin und Padding

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
    padding-left: 50px;
    padding-right: 50px;
    padding-top: 50px;
    padding-bottom: 50px;
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
<div class="hintergrund-rot text-weiss padding-50 margin-obenunten-20">
    <h1>Über uns</h1>
    <p>Das ist ein weiterer Abschnitt</p>
</div>
```

{: .task }
Experimentiere heraus, wie du das neu gelernte am Besten in deinem Projekt verwenden kannst.