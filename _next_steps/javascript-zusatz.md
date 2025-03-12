---
layout: post
title:  JavaScript Zusatz
nav_order: 2
---

# JavaScript Zusatz

## Prompts

Was ist, wenn wir den Nutzer dazu auffordern wollen, eine Eingabe zu machen? Dafür können wir ein `prompt` verwenden. Ein `prompt` ist ein Dialogfenster, das eine Nachricht anzeigt und den Benutzer auffordert, eine Eingabe zu machen. 

<div class="code-example">
<button onclick="halloPromptOnly()">Hallo</button>
</div>

`script.js`
```javascript
function hallo() {
    prompt("Wie heißt du?");
}
```

`index.html`
```html
<button onclick="hallo()">Hallo</button>
```

Noch besser ist es, wenn wir die Eingabe speichern und sie später verwenden können. Dafür können wir die Eingabe in einer Variable speichern. Eine Variable ist ein Container, in dem wir Werte speichern können. Stell dir eine Variable wie eine Schachtel vor, in der du Dinge aufbewahren kannst. In der Mathematik ist eine Variable ein Symbol, das einen Wert repräsentiert, zum Beispiel `x` oder `y`.

<div class="code-example">
<button onclick="halloAlertName()">Hallo</button>
</div>

```javascript
function hallo() {
    var name = prompt("Wie heißt du?");
    alert(name);
}
```

## Informationen abfragen



Bisher zeigen wir nur den Namen an. 

Wir können auch Texte mit Variablen kombinieren, zum Beispiel so:

<div class="code-example">
<button onclick="halloAlertNameFull()">Hallo</button>
</div>

```javascript
function hallo() {
    var name = prompt("Wie heißt du?");
    alert("Hallo " + name + "!");
}
```

In diesem Beispiel wird der Text "Hallo" mit dem Namen des Benutzers kombiniert. Das `+` Zeichen wird verwendet, um zwei Texte zu verbinden.

## Eingabe überprüfen

Manchmal möchten wir überprüfen, ob der Benutzer eine Eingabe gemacht hat. Dafür können wir eine `if`-Anweisung verwenden. Eine `if`-Anweisung führt einen Block von Code aus, wenn eine Bedingung wahr ist.

```
if (es regnet) {
    Regenjacke anziehen
} else {
    Sonnenbrille aufsetzen
}
```

In diesem Beispiel wird überprüft, ob es regnet. Wenn es regnet, wird die Regenjacke angezogen. Andernfalls wird die Sonnenbrille aufgesetzt.

Die selbe Logik können wir auch für die Eingabe des Benutzers verwenden. Das `===` Zeichen wird verwendet, um zwei Werte zu vergleichen. Wenn die Eingabe des Benutzers gleich "1847" ist, wird "Richtig!" angezeigt. Andernfalls wird "Falsch!" angezeigt.

<div class="code-example">
In welchem Jahr wurde Hapag-Lloyd gegründet? <button onclick="pruefeAntwort()">Antwort prüfen</button>
</div>

```javascript
function pruefeAntwort() {
    var antwort = prompt("In welchem Jahr wurde Hapag-Lloyd gegründet?");
    if (antwort === "1847") {
        alert("Richtig!");
    } else {
        alert("Falsch!");
    }
}
```


<script>
function halloPromptOnly() {
    prompt("Wie heißt du?");
}

function halloAlertName() {
    var name = prompt("Wie heißt du?");
    alert(name);
}

function halloAlertNameFull() {
    var name = prompt("Wie heißt du?");
    alert("Hallo " + name + "!");
}

function pruefeAntwort() {
    var antwort = prompt("In welchem Jahr wurde Hapag-Lloyd gegründet?");
    if (antwort === "1847") {
        alert("Richtig!");
    } else {
        alert("Falsch!");
    }
}
</script>