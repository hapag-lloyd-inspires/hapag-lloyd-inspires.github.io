---
layout: post
title:  Bilder einfügen
nav_order: 9
---
<style>
.tiger-bild {
width: 200px;
}

.bild-small {
    width: 50px;
}

.bild-medium {
    width: 200px;
}

.bild-large {
    width: 400px;
}

.rahmen-1 {
border-color: rgb(44, 132, 250);
border-width: 5px;
border-style: solid;
}

.rahmen-2 {
border-color: rgb(250, 44, 123);
border-width: 3px;
border-style: dashed;
}
</style>
# Bilder einfügen

Bilder sind ein wichtiger Bestandteil des Designs einer Webseite. Sie können das Erscheinungsbild einer Webseite stark beeinflussen. 

Bilder können mit dem `<img>` Element in HTML eingefügt werden. Das `<img>` Element hat zwei erforderliche Attribute: `src` und `alt`. 

Das `src` Attribut gibt den Pfad zum Bild an, während das `alt` Attribut eine alternative Beschreibung des Bildes bereitstellt. Das `alt` Attribut ist wichtig für die Barrierefreiheit von Webseiten, da es von Screenreadern verwendet wird, um das Bild zu beschreiben.

Ein Beispiel:

<div class="code-example">
<img src="hund.jpg" alt="Ein Bild von einem Hund">
</div>

```html
<img src="hund.jpg" alt="Ein Bild von einem Hund">
```

Huch! Das Bild wird nicht angezeigt. Was ist passiert? Das Bild `bild.jpg` existiert nicht, und stattdessen wird der Text, der im `alt` Attribut angegeben ist, angezeigt.

Was müssen wir nun machen? Zuerst können wir uns ein Bild aus dem Internet heraussuchen und es herunterladen. Folgende Webseite bietet kostenlose Bilder an: 
- [Unsplash](https://unsplash.com/)
- [Pexels](https://www.pexels.com/)
- [Pixabay](https://pixabay.com/)
- [Lorem Picsum](https://picsum.photos/)

Als nächstes müssen wir das Bild in unser Projekt hochladen. Dazu klicken wir auf die drei Punkte in der linken Seitenleiste und wählen `Datei hochladen`. Anschließend wählen wir das Bild aus und klicken auf `Öffnen`.

![upload-images.png](/images/upload-images.png)

In der Dateiübersicht können wir das Bild sehen. 

![image-in-files.png](/images/image-in-files.png)

<div class="code-example">
<img src="tiger.jpg" alt="Ein Bild von einem Tiger">
</div>

```html
<img src="tiger.jpg" alt="Ein Bild von einem Tiger">
```

{: .task }
> 1. Lade ein Bild in dein Projekt hoch.
> 2. Erstelle ein `<img>` Element in deiner `index.html` Datei und füge das Bild hinzu.

## Die Größe von Bildern ändern

Bilder können mit CSS formatiert werden, um ihre Größe, Ausrichtung und andere Eigenschaften zu ändern.

Ein Beispiel:

<div class="code-example">
<style>
.tiger-bild {
    width: 200px;
}
</style>

<img class="tiger-bild" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >

</div>

`style.css`
```css
.tiger-bild {
    width: 200px;
}
```

`index.html`
```html
<img class="tiger-bild" src="tiger.jpg" alt="Ein Bild von einem Tiger">
```

Wir können verschiedene Klassen erstellen, um die Größe des Bildes zu ändern. Zum Beispiel können wir eine Klasse erstellen, die das Bild größer oder kleiner macht.

<div class="code-example">
<img class="bild-small" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >
<img class="bild-medium" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >
<img class="bild-large" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >
</div>

`style.css`
```css
.bild-small {
    width: 50px;
}
.bild-medium {
    width: 200px;
}
.bild-large {
    width: 400px;
}
```

`index.html`
```html
<img class="bild-small" src="tiger.jpg" alt="Ein Bild von einem Tiger">
<img class="bild-medium" src="tiger.jpg" alt="Ein Bild von einem Tiger">
<img class="bild-large" src="tiger.jpg" alt="Ein Bild von einem Tiger">
```


{: .task }
> 1. Füge noch drei weitere Bilder in deinem Projekt hinzu.
> 2. Erstelle Klassen in deiner `style.css` Datei, um die Größe der Bilder zu ändern.
> 3. Füge die Klassen zu den Bildern hinzu, um die Größe der Bilder zu ändern. 
> 4. Erstelle eine Klasse `bild-extrem-gross` und füge sie zu einem der Bilder hinzu. Experimentiere mit der Größe des Bildes.


## Rahmen um Bilder

Bilder können mit CSS auch mit einem Rahmen versehen werden. Ein Rahmen kann das Bild hervorheben und ihm einen stilvollen Look verleihen.

Ein Beispiel:

<div class="code-example">

<img class="tiger-bild rahmen-1" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >
<img class="tiger-bild rahmen-2" src="/images/tiger.jpg" alt="Ein Bild von einem Tiger" >

</div>

`style.css`
```css
.tiger-bild {
    width: 200px;
}

.rahmen-1 {
    border-color: rgb(44, 132, 250);
    border-width: 5px;
    border-style: solid;
}

.rahmen-1 {
    border-color: rgb(250, 44, 123);
    border-width: 3px;
    border-style: dashed;
}
```
`index.html`
```html
<img class="tiger-bild rahmen-1" src="tiger.jpg" alt="Ein Bild von einem Tiger" class="img">
```

{: .task }
> 1. Füge eine Klasse in deiner `style.css` Datei hinzu, die einen Rahmen um das Bild hinzufügt.
> 2. Füge das Bild in deinem Projekt hinzu und füge die Klasse hinzu, um einen Rahmen um das Bild zu erstellen.
> 3. Experimentiere mit der `border-style` css Eigenschaft. Welche anderen Rahmenstile gibt es? (Tipp: gehe auf [w3schools](https://www.w3schools.com/cssref/pr_border-style.asp) um mehr über die `border-style` Eigenschaft zu erfahren.)

{: .extra-task }
Was passiert, wenn du statt der Breite in Pixel (`px`) eine andere Einheit wie Prozent (`%`) verwendest? Zum Beispiel `width: 50%;`. Was passiert, wenn du die Breite des Browsers oder der Vorschau änderst?

{: .extra-task }
Finde heraus, was die css Regeln `min-width: 100px;` und `max-width: 500px;` bedeuten. Wie kannst du diese Regeln in deinem Projekt verwenden?
