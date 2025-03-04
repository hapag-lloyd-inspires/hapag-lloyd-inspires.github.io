---
layout: post
title:  Listen und Links
nav_order: 3
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

Links werden mit dem `<a>` (*"anchor"*) Tag erstellt. Das `href` (*"hypertext reference"*) Attribut gibt die URL der verlinkten Seite an.

<div class="code-example py-7">
<p>
Hapag-Lloyd ist ein Unternehmen, das sich auf den Transport von Containern spezialisiert hat. 
Mehr Informationen <a href="https://www.hapag-lloyd.com">hier</a>.
</p>
</div>
```html
<p>
Hapag-Lloyd ist ein Unternehmen, das sich auf den Transport von Containern spezialisiert hat. 
Mehr Informationen <a href="https://www.hapag-lloyd.com">hier</a>.
</p>
```
![img.png](/images/replit-open-new-tab.png)

Um Links zu einer anderen Webseite zu öffnen solltest den Webview in einem neuen Tab öffnen. Klicke dazu auf den Knop "New Tab" oben rechts in der Vorschau.

{: .task }
Erstelle drei Links zu Webseiten, die Informationen über dein Thema enthalten.

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
