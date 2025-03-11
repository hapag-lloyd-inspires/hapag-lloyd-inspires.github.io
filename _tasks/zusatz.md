---
layout: post
title:  Zusatz
nav_order: 20
---
<style>
.knopf {
    display: inline-block; /* Damit der Knopf nicht die ganze Breite einnimmt */
    padding: 10px 20px;
    color: #fff;
    text-decoration: none; /* Entfernt die Unterstreichung */
}

.background-blue {
background: #5a82ef;
}

.runde-ecken {
    border-radius: 15px; 
}

.knopf-mit-rahmen {
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
    border-color: #5a82ef;
    border-width: 1px;
    border-style: solid;
}
</style>
# Zusatz

## Knöpfe
### Knöpfe erstellen
In diesem Abschnitt lernst du wie du Knöpfe in deine Webseite einfügen kannst.

<div class="code-example py-7">

<a href="https://www.google.com" class="knopf background-blue">Google</a>
</div>

`style.css`
```css
.knopf {
    display: inline-block; /* Damit der Knopf nicht die ganze Breite einnimmt */
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
    background: #5a82ef;
    color: #fff;
    text-decoration: none; /* Entfernt die Unterstreichung */
}
.background-blue {
    background: #5a82ef;
}
```
`index.html`
```html
<a href="https://www.google.com" class="knopf background-blue">Google</a>
```

{: .task }
> 1. Füge einen Knopf zu deiner Webseite hinzu.
> 2. Ändere den Text des Knopfes und die URL, zu der der Knopf verlinkt.
> 3. Ändere die Farbe des Knopfes.



### Knöpfe mit runden Ecken
Das Ergebnis ist ein Knopf, der auf die Google Webseite verlinkt. Wir können aber noch mehr machen, zum Beispiel die Ecken des Knopfes abrunden. Dazu fügen wir eine weitere Klasse in die `style.css` Datei hinzu und fügen diese Klasse dem `class=` Attribut unseres `<a>` Elements hinzu.

<div class="code-example py-7">
<a href="https://www.google.com" class="knopf background-blue runde-ecken">Google</a>
</div>
`index.html`

```html
<a href="https://www.google.com" class="knopf runde-ecken">Google</a>
```

`style.css`
```css
.knopf {
    display: inline-block; /* Damit der Knopf nicht die ganze Breite einnimmt */
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #fff;
    text-decoration: none; /* Entfernt die Unterstreichung */
}

.background-blue {
    background: #5a82ef;
}

.runde-ecken {
    border-radius: 15px; 
}
```

{: .task }
Erstelle einen Knopf mit abgerundeten Ecken. Du kannst die Größe der Ecken ändern, indem du den Wert von `border-radius` änderst.

### Knöpfe nur mit Rahmen

<div class="code-example py-7">
<a href="https://www.google.com" class="runde-ecken knopf-mit-rahmen">Google</a>
</div>

`style.css`
```css
.runde-ecken {
    border-radius: 15px; 
}
.knopf-mit-rahmen {
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
    border-color: #5a82ef;
    border-width: 1px;
    border-style: solid;
}
```

`index.html`
```html
<a href="https://www.google.com" class="knopf runde-ecken">Google</a>
```


### Knöpfe mit Hover-Effekt
Ein weiteres Feature, das wir hinzufügen können, ist ein Hover-Effekt. Wenn der Mauszeiger über den Knopf bewegt wird, ändert sich die Farbe des Knopfes. Dazu fügen wir `:hover` in die `style.css` Datei hinzu.

`style.css`
```css
...
.knopf:hover {
    background: #4a6cd4;
}
```

{: .task }
Füge einen Hover-Effekt zu deinem Knopf hinzu.
