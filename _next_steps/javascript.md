---
layout: post
title:  JavaScript Quiz
nav_order: 1
---

# JavaScript

JavaScript ist eine der drei Kern-Technologien des World Wide Web. Es wird verwendet, um Webseiten interaktiv zu gestalten und dynamische Inhalte zu erstellen. In dieser Aufgabe lernst du, wie du JavaScript in deine Webseite einbindest und einfache Interaktionen hinzufügst.

## Alerts

Ein Alert ist ein Dialogfenster, das eine Nachricht anzeigt. Ein Alert wird mit der `alert()` Funktion erstellt. Die Funktion nimmt eine Nachricht als Argument an, die im Dialogfenster angezeigt wird.

`script.js`
```javascript
alert("Hallo Welt!");
```

{: .task }

Erstelle ein Alert-Fenster, das eine Nachricht anzeigt.

## Richt-Falsch Quiz

Mit dem `onclick`-Attribut können Funktionen ausgeführt werden, wenn ein Element geklickt wird. Das, was in den Anführungszeichen steht, wird als JavaScript-Code ausgeführt.

<div class="code-example">
<p>Richtig oder Falsch: H4 steht für "Hyper Text Markup Language".</p>
<ul>
    <li><button onclick="alert('falsch')">Wahr</button></li>
  <li><button onclick="alert('richtig')">Falsch</button></li>
</ul>

</div>

`index.html`
```html
<p>Richtig oder Falsch: H4 steht für "Hyper Text Markup Language".</p>
<ul>
    <li><button onclick="alert('falsch')">Wahr</button></li>
  <li><button onclick="alert('richtig')">Falsch</button></li>
</ul>
```

Warum verwenden wir `'` und nicht `"`? Wenn wir `"`verwenden würden, dann würde der Browser denken, dass der String endet, wenn er das nächste `"` sieht. Anders gesagt würde er denken, dass das `onclick` Attribut bereits zuende ist. 

{: .task }

Erstelle ein Richt-Falsch Quiz mit einer Frage und zwei Antwortmöglichkeiten. Wenn der Benutzer auf eine Antwort klickt, wird ein Alert-Fenster mit der Antwort angezeigt.

## Multiple Choice Quiz

Wir können auch mehrere Antwortmöglichkeiten in einem Quiz haben. Hier ist ein Beispiel:

<div class="code-example">
  <h4>Mein Quiz</h4>
  <ol>
    <li><button onclick="alert('falsch')">a</button></li>
    <li><button onclick="alert('falsch')">b</button></li>
  <li><button onclick="alert('richtig')">c</button></li>
    <li><button onclick="alert('falsch')">d</button></li>

  </ol>
</div>

`index.html`
```html
<h4>Mein Quiz</h4>
<ol>
  <li><button onclick="alert('falsch')">a</button></li>
  <li><button onclick="alert('falsch')">b</button></li>
  <li><button onclick="alert('richtig')">c</button></li>
  <li><button onclick="alert('falsch')">d</button></li>
</ol>
```

{: .task }

Erstelle ein Multiple Choice Quiz mit einer Frage und vier Antwortmöglichkeiten. Wenn der Benutzer auf eine Antwort klickt, wird ein Alert-Fenster mit der Antwort angezeigt.

## Hintergrundfarbe ändern

Mit JavaScript können wir auch die Hintergrundfarbe der Webseite ändern. Wir können dies mit dem `style`-Attribut und der `backgroundColor` Eigenschaft tun.

`document.body` bezieht sich auf das `<body>` Element der Webseite. Leider funktioniert diese Logik nicht mit anderen html Elementen. 

<div class="code-example">
<button onclick="document.body.style.backgroundColor = 'lightblue'">Blau</button>
<button onclick="document.body.style.backgroundColor = 'lightgreen'">Grün</button>
<button onclick="document.body.style.backgroundColor = 'lightcoral'">Rot</button>
<button onclick="document.body.style.backgroundColor = 'initial'">weiß</button>

</div>

`index.html`
```html
<button onclick="document.body.style.backgroundColor = 'lightblue'">Blau</button>
<button onclick="document.body.style.backgroundColor = 'lightgreen'">Grün</button>
<button onclick="document.body.style.backgroundColor = 'lightcoral'">Rot</button>
<button onclick="document.body.style.backgroundColor = 'white'">weiß</button>
```

## Funktionen

Eine Funktion ist ein Block von Code, der eine bestimmte Aufgabe ausführt. Funktionen werden mit dem `function` Schlüsselwort erstellt.

<div class="code-example">
<button onclick="greet()">Klick mich!</button>
</div>

`script.js`
```javascript
function greet() {
    alert("Hallo Welt!");
}
```

```html
<button onclick="greet()">Klick mich!</button>
```

{: .task }

Erstelle eine Funktion, die ein Alert-Fenster mit einer Nachricht anzeigt. Füge einen Button hinzu, der die Funktion ausführt.

Warum erstellen wir Funktionen? Funktionen helfen uns, unseren Code zu organisieren und zu strukturieren. Wenn wir denselben Code an mehreren Stellen verwenden, können wir ihn in eine Funktion auslagern und ihn an verschiedenen Stellen aufrufen. Wir können auch mehrere Befehle in eine Funktion schreiben und sie zur selben Zeit ausführen:

<div class="code-example">
<button onclick="greet2()">Klick mich!</button>
</div>

`script.js`
```javascript
function greet() {
    document.body.style.backgroundColor = 'lightblue';
    alert("Hallo Welt!");
}
```

{: .task }

Erstelle drei Buttons, die die Hintergrundfarbe der Webseite ändern. Jeder Button sollte eine andere Farbe setzen.

## Alles zusammen

<div class="code-example">
<h4>Mein Quiz</h4>
 <ol>
    <li><button onclick="falsch()">a</button></li>
    <li><button onclick="falsch()">b</button></li>
  <li><button onclick="richtig()">c</button></li>
  </ol>

</div>

`script.js`
```javascript
function falsch() {
  document.body.style.backgroundColor = 'red';
  alert('falsch')
}

function richtig() {
  alert('richtig');
  document.body.style.backgroundColor = 'green';
}
```

`index.html`
```html
<h4>Mein Quiz</h4>
 <ol>
    <li><button onclick="alert('falsch')">a</button></li>
    <li><button onclick="alert('falsch')">b</button></li>
  <li><button onclick="alert('richtig')">c</button></li>
  </ol>
```

{: .task }

Erstelle ein Quiz mit einer Frage und vier Antwortmöglichkeiten. Wenn der Benutzer auf eine Antwort klickt, wird ein Alert-Fenster mit der Antwort angezeigt und die Hintergrundfarbe der Webseite ändert sich je nach Antwort. Verwende Funktionen, um die Antwort und die Hintergrundfarbe zu ändern.

<script>
    function falsch() {
      document.body.style.backgroundColor = 'lightcoral';
      alert('falsch')
    }

    function richtig() {
      alert('richtig');
      document.body.style.backgroundColor = 'lightgreen';
    }

function greet() {
    alert("Hallo Welt!");
}

function greet2() {
document.body.style.backgroundColor = 'lightblue';
    alert("Hallo Welt!");
}
</script>