---
layout: post
title:  Listen und Links
nav_order: 4
---

# Listen und Links

## Listen

Listen sind eine Möglichkeit, Informationen in einer geordneten oder ungeordneten Weise darzustellen.

### Ungeordnete Liste

Eine ungeordnete Liste wird mit dem `<ul>` (*"unordert list"*) Tag erstellt. Jeder Punkt in der Liste wird mit dem `<li>` (*"list item"*) Element erstellt.

<div class="code-example">
Folgende Programmiersprachen werden bei Hapag-Lloyd benutzt:
<ul>
  <li>html und css</li>
  <li>Java</li>
  <li>Python</li>
</ul>
</div>

```html
Folgende Programmiersprachen werden bei Hapag-Lloyd benutzt:
<ul>
  <li>html und css</li>
  <li>Java</li>
  <li>Python</li>
</ul>
```

{: .task }
Erstelle eine ungeordnete Liste welche Fakten über dein Thema enthält.

### Geordnete Listen

Statt einer ungeordneten Liste kannst du auch eine geordnete Liste verwenden. Statt des `<ul>` Elements verwendet man das `<ol>` Element (*"ordered list"*). 

{: .task }
Erstelle eine geordnete Liste über dein Thema.

Geordnete Listen sind automatisch nummeriert. Wenn du die Reihenfolge der Elemente änderst, ändert sich auch die Nummerierung.

{: .task }
Probiere aus, die Reihenfolge der Elemente in deiner geordneten Liste zu ändern.

## Links

Links sind eine Möglichkeit, von einer Webseite zu einer [anderen Webseite](https://www.w3schools.com) zu navigieren. 

Links werden mit dem `<a>` (*"anchor"*) Tag erstellt. 

<div class="code-example py-7">
<p>
Die Webseite von Apple ist <a>apple.com</a>
</p>
</div>
```html
<p>
Die Webseite von Apple ist <a>apple.com</a>
</p>
```

{: .task }
Erstelle einen Link zu einer Webseite, die Informationen über dein Thema enthält.

Hmm, noch können wir nicht auf die Webseite klicken. Das liegt daran, dass wir den Link noch nicht mit einer URL verknüpft haben.

Das `href` Attribut wird verwendet, um die URL des Links anzugeben. Das, was zwischen den `<a>` Tags steht, ist lediglich der Text, der auf der Webseite angezeigt wird.

<div class="code-example py-7">
<p>
Die Webseite von Apple ist <a href="https://www.apple.com">apple.com</a>
</p>
<p>
    Die Webseite von Google ist <a href="https://www.google.com">hier</a>
</p>
</div>

```html
<p>
Die Webseite von Apple ist <a href="https://www.apple.com">apple.com</a>
</p>
<p>
    Die Webseite von Google ist <a href="https://www.google.com">hier</a>
</p>
```

{: .task }
Erstelle drei Links zu Webseiten, die Informationen über dein Thema enthalten. Überprüfe, ob die Links funktionieren.


## Links in Listen

Links können auch in Listen verwendet werden.

<div class="code-example">
Eine Webseite besteht aus folgenden Technologien:
<ul>
  <li>Hyper-Text Markup Language - <a href="https://developer.mozilla.org/de/docs/Web/HTML">html</a></li>
  <li>Cascardian Style Sheet - <a href="https://developer.mozilla.org/de/docs/Web/CSS">W3Schools</a></li>
  <li>JavaScript - <a href="https://developer.mozilla.org/de/docs/Web/JavaScript">JavaScript</a></li>
</ul>
</div>

```html
Eine Webseite besteht aus folgenden Technologien:
<ul>
  <li>Hyper-Text Markup Language - <a href="https://developer.mozilla.org/de/docs/Web/HTML">html</a></li>
  <li>Cascardian Style Sheet - <a href="https://developer.mozilla.org/de/docs/Web/CSS">W3Schools</a></li>
  <li>JavaScript - <a href="https://developer.mozilla.org/de/docs/Web/JavaScript">JavaScript</a></li>
</ul>
```

{: .task }
Erstelle eine Liste mit Links zu Webseiten, die Informationen über dein Thema enthalten.

{: .extra-task }
Erstelle eine Liste, welche fette, kursiv und fett und kursiv geschriebene Datenpunkte enthält. Ein Beispiel siehst du unter der Aufgabe.

<div class="code-example">
<ul>
  <li><span style="font-style: italic;">html</span></li>
  <li><span style="font-weight: bold; ">W3Schools</span></li>
  <li><span style="font-weight: bold; font-style: italic;">JavaScript</span></li>
</ul>
</div>