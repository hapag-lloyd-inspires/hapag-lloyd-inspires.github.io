---
layout: post
title:  "1. Texte Stylen"
nav_order: 2
---
# Intro zu repl.it und Texte stylen

## Aufgabe 1: erstelle ein Repl.it
1. Gehe auf [replit.com](https://www.replit.com) 
2. erstelle einen Account 
3. erstelle ein neues REPL

## Aufgabe 2: Texte stylen

Im folgenden wirst du einen Steckbrief über ein Thema deiner Wahl erstellen. Suche dir jetzt ein Thema aus und schreibe einen kurzen Text darüber. Du kannst mit einer Suchmaschine oder auf Wikipedia auch Absätze kopieren.

### Überschriften und Absätze
1. Erstelle eine neue Datei und nenne sie `index.html`
2. Füge eine Überschrift hinzu. Verwende dazu den `<h1></h1>` tag.
3. Füge deinem Text Abschnitte hinzu. Verwende dazu den `<p></p>` tag.
4. ein Absatz braucht Überschriften. Füge Absatzüberschriften hinzu. Verwende dazu die Tags `h2`, `h3`, `h4`, `h5` und `h6`.
Zum Beispiel:
{% highlight html %}
<h1>Haupüberschrift</h1>
<h2>Unterüberschrift</h2>
<p>Das ist ein Absatz</p>
<p>Das ist ein weiterer Absatz</p>
<h3>Unterunterüberschrift</h3>
<p>Das ist ein Absatz</p>
<h3>Unterunterüberschrift</h3>
<p>Das ist ein Absatz</p>

{% endhighlight %}

Erstelle eine Liste. Verwende dazu den `<ul></ul>` tag für eine ungeordnete Liste und den `<ol></ol>` tag für eine geordnete Liste.
{% highlight html %}
<ul>
  <li>Erster Punkt</li>
  <li>Zweiter Punkt</li>
</ul>
{% endhighlight %}

Füge deinem Text Bilder hinzu. Verwende dazu den `<img>` tag.
{% highlight html %}

<img src="bild.jpg" alt="Beschreibung des Bildes">
{% endhighlight %}

Füge deinem Text Zitate hinzu. Verwende dazu den `<blockquote></blockquote>` tag.


### Text stylen


Schreibe Text kursiv oder fett. Verwende dazu die css Eigenschaften `font-style` und `font-weight`.
{% highlight html %}
<p style="font-style: italic;">Das ist ein kursiver Absatz</p>
<p style="font-weight: bold;">Das ist ein fetter Absatz</p>
{% endhighlight %}


### Farbe
todo
{: .label .label-yellow }
> Farben erklären

Hebe Text hervor, als wäre er mit einem Textmarker markiert. Verwende dazu die css-Eigenschaft `background-color`.
Unterstreiche Text.
Streiche Text durch


Füge deinem Text Farbe hinzu. Verwende dazu das `style`-Attribut.
{% highlight html %}
<p style="color: red;">Das ist ein roter Absatz</p>
{% endhighlight %}

Unterstreiche Text und mach ihn kursiv und fett und blau zur selben Zeit.
<div>
<p>Das ist <span style="font-style: italic; font-weight: bold; text-decoration: underline; background-color: #7be2f9">cooler</span> Text.</p>
</div>
{:  .p-4 .text-center }

### Ausrichtung


text-align: center right  left
{: .highlight }

### Links
Füge deinem Text Links hinzu. 
1. Erstelle zuerst eine neue Datei, zum Beispiel `kontakt.html`
2. Jetzt hast du zwei Dateien, `index.html` und `kontakt.html`. Verlinke die beiden Dateien miteinander. Verwende dazu den Tag `<a href="kontakt.html">Kontakt</a>`.
3. Erstelle eine zweite Datei und verlinke auch auf sie.
4. Verlinke auch auf externe Seiten, zum Beispiel auf die [Wikipedia-Seite von BMW](https://de.wikipedia.org/wiki/BMW)


- hover
- div & padding, margin, border, align
- layout
- 
<details open markdown="block">
  <summary>
Hinweis

</summary>
{% highlight html %}
<h1>Überschrift 1</h1>
{% endhighlight %}
</details>
