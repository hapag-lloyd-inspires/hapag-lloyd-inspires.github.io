---
layout: post
title:  JavaScript Zusatz
nav_order: 22
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

<script>
function halloPromptOnly() {
    prompt("Wie heißt du?");
}

function halloAlertName() {
    var name = prompt("Wie heißt du?");
    alert(name);
}
</script>