---
layout: post
title:  Absätze und Überschriften
nav_order: 2
---

# Strukturieren von Texten

## Struktur einer html Seite

Im vorherigen Schritt haben wir ein neues Projekt erstellt und eine Vorschau erstellt. Dabei hast du drei Dateien erstellt:
- `index.html`
- `style.css`
- `script.js`

Wir wollen uns jetzt auf die `index.html` Datei konzentrieren. Die `index.html` Datei ist die Startseite deiner Webseite. Hier wird der Inhalt deiner Webseite angezeigt. Bisher sieht sie folgendermaßen aus:

<div class="code-example py-7">
Hello world
</div>

```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  Hello world
  <script src="script.js"></script>
</body>

</html>
```

Folgende Elemente siehst du in der `index.html` Datei:
- `<!DOCTYPE html>`: Dieses Element gibt an, dass es sich um eine HTML-Datei handelt.
- `<html>`: Dieses Element ist das Wurzelelement und umschließt den gesamten Inhalt der Webseite.
- `<head>`: Dieses Element enthält Metadaten über das Dokument, wie z.B. den Titel der Webseite und Verweise auf externe Dateien.
- `<title>`: Dieses Element gibt den Titel der Webseite an, der im Browser-Tab angezeigt wird.
- `<link>`: Dieses Element verweist auf eine externe Datei, in diesem Fall auf die `style.css` Datei. Dazu später mehr.
- `<body>`: Dieses Element enthält den eigentlichen Inhalt der Webseite, wie Texte, Bilder und Links.


## Texte ändern

Das `<body>` Element enthält bisher nur den Text "Hello world". Ändern wir das.

<div class="code-example py-7">
Hallo Hackerschool!
</div>

```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>replit</title>
  <link href="style.css" rel="stylesheet" type="text/css" />
</head>

<body>
  Hallo Hackerschool!
  <script src="script.js"></script>
</body>

</html>
```

Sobald du den Text geändert hast, klicke auf den "Refresh" Knopf in der Vorschau um die Änderungen zu sehen.

![replit-refresh.png](/images/replit-refresh.png)

{: .task }
> 1. Ändere den Text im `<body>` Element.
> 2. Klicke auf den grünen `Run` Button um die Änderungen zu sehen.

## Ein Text über ein Thema einfügen

Während der nächsten zwei Tage ist es deine Aufgabe, eine Webseite zu erstellen, welches ein Thema deiner Wahl vorstellt. Du kannst zum Beispiel eine Webseite über deine Lieblingsband, dein Lieblingsessen oder ein Hobby erstellen.

<div class="code-example">
  Hapag-Lloyd
  Die Hapag-Lloyd AG ist ein Transport- und Logistikunternehmen mit Unternehmenssitz in Hamburg.

Gegründet 1847 - geh mit uns auf Zeitreise
Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.
Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.

Unsere Werte
„We care. We move. We deliver.“ – das sind unsere Unternehmenswerte, und sie stehen im Mittelpunkt unseres Handelns. Unsere Werte erzählen eine Geschichte darüber, woher wir kommen. Sie definieren, wer wir sind, und sie leiten uns auf unserem Weg in die Zukunft.
</div>
```html
...
<body>
  Hapag-Lloyd
  Die Hapag-Lloyd AG ist ein Transport- und Logistikunternehmen mit Unternehmenssitz in Hamburg.

  Gegründet 1847 - geh mit uns auf Zeitreise
  Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.
  
  Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.

  Unsere Werte
  „We care. We move. We deliver.“ – das sind unsere Unternehmenswerte, und sie stehen im Mittelpunkt unseres Handelns. 
  
  Unsere Werte erzählen eine Geschichte darüber, woher wir kommen. Sie definieren, wer wir sind, und sie leiten uns auf unserem Weg in die Zukunft.

  <script src="script.js"></script>
</body>
...
```

Hmm, das sieht noch nicht so gut aus. Wir müssen den Text strukturieren, dazu gleich mehr.

{: .task }
> 1. Suche dir ein Thema aus.
> 2. Kopiere einen Text über das Thema von Wikipedia oder einer anderen Webseite.
> 3. Füge den Text in die `index.html` Datei in das `<body>` Element ein.

{: .important }
Verwende für das Kopieren des Textes jetzt maximal **5 Minuten**. Du kannst den Text später noch anpassen und erweitern.

## Überschriften

Mit den Elementen `<h1>`, `<h2>`, `<h3>` kannst du Überschriften hinzufügen. Die `<h1>` Überschrift ist die Hauptüberschrift und sollte nur einmal pro Seite verwendet werden. Die `<h2>` Überschrift ist die Unterüberschrift und kann mehrmals verwendet werden.

<div class="code-example">
  <h1>Hapag-Lloyd</h1>
  Die Hapag-Lloyd AG ist ein Transport- und Logistikunternehmen mit Unternehmenssitz in Hamburg.

<h2>Gegründet 1847 - geh mit uns auf Zeitreise</h2>
Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.

Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.

<h2>Unsere Werte</h2>
„We care. We move. We deliver.“ – das sind unsere Unternehmenswerte, und sie stehen im Mittelpunkt unseres Handelns.

Unsere Werte erzählen eine Geschichte darüber, woher wir kommen. Sie definieren, wer wir sind, und sie leiten uns auf unserem Weg in die Zukunft.

</div>
```html
...
<body>
  <h1>Hapag-Lloyd</h1>
  Die Hapag-Lloyd AG ist ein Transport- und Logistikunternehmen mit Unternehmenssitz in Hamburg.

  <h2>Gegründet 1847 - geh mit uns auf Zeitreise</h2>
  Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.
  
  Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.

  <h2>Unsere Werte</h2>
  „We care. We move. We deliver.“ – das sind unsere Unternehmenswerte, und sie stehen im Mittelpunkt unseres Handelns.

  Unsere Werte erzählen eine Geschichte darüber, woher wir kommen. Sie definieren, wer wir sind, und sie leiten uns auf unserem Weg in die Zukunft.

  <script src="script.js"></script>
</body>
...
```
Das sieht schon etwas besser aus. Wenn du genau hinschaust, dann siehst du, dass der Text noch nicht so gut lesbar ist. Wir können den Text noch weiter strukturieren, indem wir Absätze hinzufügen.

{: .task }
>Füge folgendes deinem Text hinzu:
> 1. eine Hauptüberschrift (verwende das `<h1>` Element)
> 2. mindestens zwei Unterüberschriften (verwende das `<h2>` Element.)
> 3. mindestens zwei Abschnittsüberschriften (verwende das `<h3>` Element)

{: .extra-task }
Finde heraus, bis zu welcher `<h...>` Ebene du Überschriften verwenden kannst!


## Absätze

<div class="code-example">
  <h2>Gegründet 1847 - geh mit uns auf Zeitreise</h2>
  <p>Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.</p>

  <p>Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.</p>
</div>

```html
...
  <h2>Gegründet 1847 - geh mit uns auf Zeitreise</h2>
  <p>Die Wurzeln der Hapag-Lloyd AG reichen bis weit ins 19. Jahrhundert zurück, als die Gründungsgesellschaften Hamburg-Amerikanische Packetfahrt-Actien-Gesellschaft (Hapag) und Norddeutscher Lloyd ihre ersten Schiffe mit Stückgut und Passagieren nach New York in See stechen ließen.</p>
  
  <p>Aus diesen Anfängen erwuchs in einer spannenden, an Wandlungen und Umbrüchen reichen Geschichte die führende und global agierende Containerlinienreederei, die wir heute sind.</p>
...
```

{: .task }
Füge deinem Text Absätze hinzu. Verwende dazu das `<p>` Element.

