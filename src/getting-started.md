# Loslegen

<!-- toc -->

## Installation & Updates

Bitte schau dir die Anweisungen für deinen Computer an:

- [Windows](./platform/windows/installing.md)
- [Mac](./platform/mac/installing.md)
- [Linux](./platform/linux/installing.md)

## Videos (Englisch)

Für einen schnellen Einstieg in Anki, kannst du dir diese Einführungsvideos
(auf Englisch) ansehen.
Einige wurden mit einer früheren Anki-Version erstellt, aber die Konzepte sind
dieselben.

- [Shared Decks and Review
  Basics](http://www.youtube.com/watch?v=QS2G-k2hQyg&yt:cc=on)

- [Syncing](https://www.youtube.com/watch?v=YkiM4DPzSVc&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao&yt:cc=on)

- [Switching Card
  Order](http://www.youtube.com/watch?v=DnbKwHEQ1mA&yt:cc=on)

- [Styling Cards](http://www.youtube.com/watch?v=F1j1Zx0mXME&yt:cc=on)

- [Typing in the
  Answer](http://www.youtube.com/watch?v=5tYObQ3ocrw&yt:cc=on)

Falls YouTube in deinem Land nicht verfügbar ist, kannst du die Videos stattdessen
[herunterladen](https://apps.ankiweb.net/downloads/archive/screencasts/2.0/).

## Grundlagen

### Karten

Eine Frage-Antwort-Paar heißt Karte. Das entspricht einer Karteikarte aus Papier
mit der Frage auf der Vorder- und der Antwort auf der Rückseite.
In Anki sieht eine Karte nicht wirklich wie eine Papierkarte aus, und wenn du die
Antwort anzeigen lässt, bleibt die Frage standardmäßig sichtbar.
Wenn du zum Beispiel elementare Chemie lernst, könntest du eine Karte wie die
folgende sehen:

    Frage: Elementsymbol für Sauerstoff?

Nachdem du darüber nachgedacht hast und zu dem Schluss gekommen bist, dass die
Antwort "O" ist, klickst du auf "Antwort zeigen" und siehst:

    Frage: Elementsymbol für Sauerstoff?
    Antwort: O

Nachdem du dich vergewissert hast, dass du recht hattest, kannst du Anki wissen
lassen, wie gut du dich erinnern konntest, und Anki wird entscheiden, wann es dir
die Karte das nächste Mal zeigen wird.

### Stapel

Ein Stapel is eine Gruppe von Karten. Du kannst Karten in verschiedene Stapel
aufteilen, um Teile deiner Sammlung anstatt alles auf einmal zu lernen.
Jeder Stapel kann andere Einstellungen haben, zum Beispiel wie viele neue Karten
du pro Tag sehen willst oder wie viel Abstand zwischen Wiederholungen liegen soll.

Stapel können andere Stapel enthalten, was dir erlaubt, deine Stapel in einem
Stammbaum anzuordnen. Anki benutzt "::", um verschiedene Ebenen zu trennen.
So bezeichnet ein Stapel mit dem Namen "Chinesisch::Hanzi" einen Hanzi-Stapel,
der Teil eines Chinesisch-Stapels ist. Wenn du "Hanzi" wählst, werden dir nur
Hanzi-Karten angezeigt, wenn du "Chinesisch" wählst, werden dir alle Chinesich-Karten,
inklusive der Hanzi-Karten, gezeigt.

Um einen Stapel in einem Stammbaum anzuordnen, kannst du ihm entweder einen
Namen mit "::" zwischen jeder Ebene geben oder ihn mit der Maus auf einen anderen
Stapel in der Stapelübersicht ziehen und loslassen.
Stapel, die sich in einem anderen Stapel befinden (die also mindestens ein "::"
im Namen haben), werden oft Unterstapel und Stapel der obersten Ebene
Ober- oder Elternstapel genannt. 

Anki beginnt mit einem Stapel namens Standard. Alle Karten, die irgendwie von den
anderen Stapeln getrennt wurden, landen hier. Anki versteckt den Standard-Stapel,
wenn er keine Karten enthält und du andere Stapel hinzugefügt hast.
Alternativ kannst du ihn umbenennen und für andere Karten benutzen.

Stapel werden am besten genutzt, um große Kategorien zu umfassen, und nicht spezifische
Themen wie "Essensverben" oder "Lektion 1". Für mehr Informationen dazu, siehe
bitte den Abschnitt [Stapel angemessen nutzen](editing.md#using-decks-appropriately).

Für Informationen darüber, wie Stapel die Anzeigereihenfolge von Karten beeinflussen,
siehe bitte den Abschnitt [Anzeigereihenfolge](studying.md#display-order).

### Notizen & Felder

Beim Erstellen von Karteikarten möchte man oft mehr als eine Karte
zu einer bestimmten Information zu erstellen. Wenn du zum Beispiel Französisch
lernst und behalten willst, dass "bonjour" "hallo" bedeutet, würdest du vielleicht
gerne eine Karte anlegen, die nach der deutschen Übersetzung von "bonjour" fragt,
und eine, die nach der französischen Übersetzung von "hallo" fragt.
Die erste Karte testet, ob du das fremde Wort erkennen, die zweite, ob du es
hervorrufen kannst.

Mit Papierkarteikarten ist die einzige Möglichkeit, die Informationen zweimal
aufzuschreiben, einmal für jede Karte. Einige Karteikartenprogramme erleichtern
das, indem sie die Möglichkeit bieten, Vorder- und Rückseite zu vertauschen.
Das ist eine Verbesserung, hat aber zwei große Nachteile:

- Weil solche Programme nicht separat überwachen, wie gut du eine Vokabel erkennen
  und hervorrufen kannst, werden dir die Karten nicht zum optiomalen Zeitpunkt
  gezeigt und du vergisst mehr, als dir lieb ist, oder musst mehr lernen als
  unbedingt nötig.

- Das Vertauschen von Frage und Antwort funktioniert nur, wenn du genau denselben
  Inhalt auf beiden Seiten sehen willst. Es ist dir also beispielweise nicht
  möglich, auf den Rückseiten noch Zusatzinformationen anzeigen zu lassen.

Anki löst diese Probleme, indem es dir ermöglicht, den Inhalt deiner Karten in
getrennte Informationseinheiten aufzuteilen. Anschließend kannst du Anki mitteilen,
welche Information auf welcher Karte stehen soll, und Anki kümmert sich um die
Erstellung und, wenn du später Änderungen vornimmst, Aktualisierung der Karten.

Stell dir vor, wir wollen Französischvokabeln lernen und es soll jeweils die
Seitenzahl auf der Kartenrückseite stehen. Unsere Karten sollen so aussehen:

    Frage: Bonjour
    Antwort: Hallo
       Seite 12

Und:

    Frage: Hallo
    Antwort: Bonjour
       Seite 12

In diesem Beispiel gibt es drei zusammengehörige Informationen: ein französisches
Wort, seine Bedeutung auf Deutsch und eine Seitenzahl. Zusammen sieht das so aus:

    Französisch: Bonjour
    Deutsch: Hello
    Seitenzahl: 12

In Anki heißt dieser Informationsblock *Notiz* und jede einzelne Information darin
*Feld*. Wir können also sagen, dass diese Art von Notiz drei Felder hat:
Französisch, Deutsch und Seitenzahl.

Um Felder hinzuzufügen oder zu bearbeiten, klicke während des Bearbeitens
von Notizen auf die Schaltfläche "Felder...". Für weitere Informationen siehe
bitte den Abschnitt [Felder anpassen](editing.md#customizing-fields).

### Kartentypen

Damit Anki basierend auf unseren Notizen Karten erstellen kann, müssen wir ihm
eine Blaupause zur Verfügung stellen, die besagt, welche Felder auf der Vor-
und Rückseite jeder Karte zu sehen sein sollen. Diese Blaupause heußt *Kartentyp*.
Jede Art Notiz kann einen oder mehrere Kartentypen haben. Wann immer du eine
Notiz hinzufügst, wird Anki für jeden Kartentypen eine Karte erstellen.

Jeder Kartentyp hat zwei *Vorlagen*, eine für die Frage und eine für die Antwort.
Im obigen Beispiel sollte die Karte zum Erkennen der Französischvokabel so aussehen:

    Frage: Bonjour
    Antwort: Hallo
       Seite 12

Dafür können wir die Frage- und Antwortvorlage jeweils wie folgt festlegen:

    Frage: {{Französisch}}
    Antwort: {{Deutsch}}<br>
       Seite {{Seitenzahl}}

Indem wir einen Feldnamen in doppelte geschweifte Klammern einfassen, weisen wir
Anki an, diesen Bereich mit der Information aus dem Feld zu ersetzen. Alles, was
nicht in geschweifte Klammern eingefasst ist, bleibt auf jeder Karte gleich.
So müssen wir nicht jedes Mal "Seite" in das Seitenzahl-Feld eingeben, wenn wir
Stoff hinzufügen – es wird auf jeder Karte automatisch hinzugefügt.
`<br>` ist eine besondere Zeichenfolge, die Anki anweist, die Zeile umzubrechen.
Weitere Informationen finden sich im Abschnitt [Kartenvorlagen](templates/intro.md).

Die Vorlagen für die Karte zum Hervorrufen der Vokabel funktionieren ganz ähnlich:

    Frage: {{Deutsch}}
    Antwort: {{Französisch}}<br>
       Seite {{Seitenzahl}}

Nachdem ein Kartentyp erstellt wurde, wird jedes Mal, wenn du eine neue Notiz
hinzufügst, basierend auf diesem Kartentypen eine neue Karte erstellt.
Mit Kartentypen ist es leicht, die Formatierung deiner Karten einheitlich zu
halten, und sie können den Aufwand, neue Informationen hinzuzufügen, drastisch
reduzieren.
Sie erlauben Anki auch, dafür zu sorgen, dass verwandte Karten nicht zu dicht
nacheinander erscheinen, und ermöglichen dir, einen Tippfehler oder eine
Falschinformation an einer Stelle zu korrigieren und damit alle betroffenen
Karten gleichzeitig zu aktualisieren.

Um Kartentypen hinzuzufügen oder zu bearbeiten, klicke während des Bearbeitens
von Notizen auf die Schaltfläche "Karten...". Für weitere Informationen siehe
bitte den Abschnitt [Kartenvorlagen](templates/intro.md).

### Notiztypen

Anki erlaubt dir, für unterschiedlichen Stoff verschiedene Notiztypen zu erstellen.
Jeder Notiztyp hat seine eigenen Felder und Kartentypen.
Es ist sinnvoll, für jedes weitgefasste Thema, das du lernst, einen eigenen
Notiztypen anzulegen. Im obigen Beispiel könnten wir einen Notiztypen
"Französisch" erstellen. Wenn wir dann noch Hauptstädte lernen möchten, könnten
wir dafür einen weiteren Notiztypen anlegen, der Felder wie "Land" und "Hauptstadt"
hat. 

Wenn Anki nach Duplikaten sucht, vergleicht es nur Notizen vom selben Typ.
Wenn du also eine Hauptstadt namens "Orange" hinzufügst, wirst du keine
Duplikatwarnung erhalten, wenn du irgendwann das französische Wort für "orange"
lernst.

Wenn du eine neue Sammlung anlegst, fügt Anki automatisch einige Standardnotiztypen
hinzu. Die erleichtern neuen Nutzern den Einstieg, aber auf lange Sicht wird
empfohlen, je nach dem gelernten Stoff eigene Notiztypen anzulegen.
Die Standardnotiztypen sind die folgenden:

**Einfach**  
Hat die Felder "Vorderseite" und "Rückseite" und erzeugt eine Karte.
Text, den du in die Felder eingibst, wird auf der jeweiligen Kartenseite gezeigt.

**Einfach (beide Richtungen)**  
Wie "Einfach", aber erzeugt zwei Karten für eingegebenen Text: eine von
"Vorderseite" nach "Rückseite" und eine von "Rückseite" nach "Vorderseite".

**Einfach (eine oder zwei Richtungen)**  
Erzeugt eine Karte mit "Vorderseite"→"Rückseite" und optional eine Karte mit
"Rückseite"→"Vorderseite". Dafür hat der Notiztyp ein drittes Feld namens
"Gegenrichtung hinzufügen". Wenn du irgendwelchen Text darin eingibst, wird die
umgekehrte Karte erzeugt. Mehr Informationen finden sich im Abschnitt
[Kartenvorlagen](templates/intro.md).

**Lückentext**  
Macht es einfach, Text in einen Lückentext zu verwandeln. Zum Beispiel:
"Die Mondlandung geschah im Jahre \[...\]." → "Die Mondlandung geschah im Jahre
1969." Mehr Informationen finden sich im Abschnitt
[Lückentext](editing.md#cloze-deletion).

Um deine eigenen Notiztypen hinzuzufügen und vorhandene zu bearbeiten, kannst
du vom Hauptfenster aus *Werkzeuge* > *Notiztypen verwalten* auswählen.

Notizen und Notiztypen sind dieselben für deine gesamte Sammlung und sind nicht
auf einen einzelnen Stapel beschränkt. Das bedeutet, dass du viele verschiedene
Notiztypen im selben Stapel verwenden oder Karten, die von derselben Notiz erzeugt
wurden, in verschiedene Stapel einteilen kannst.
Wenn du Notizen mithilfe des *Hinzufügen*-Fensters erstellst, kannst du auswählen,
welcher Notiztyp und welcher Stapel verwendet werden soll. Diese beiden
Entscheidungen sind komplett unabhängig voneinander.
Du kannst auch den Notiztypen von Notizen ändern,
[nachdem du sie schon erstellt hast](browsing.md).

### Sammlung

Deine Sammlung ist das gesamte in Anki gespeicherte Material – deine Karten,
Notizen, Stapel, Notiztypen, Stapeloptionen und so weiter.

## Öffentliche Stapel

Du kannst dir ein
[Video über öffentliche Stapel und Wiederholung (Englisch)](http://www.youtube.com/watch?v=QS2G-k2hQyg&yt:cc=on)
auf YouTube ansehen.

Die einfachste Möglichkeit, mit Anki loszulegen, ist, einen Stapel herunterzuladen,
den jemand geteilt:

1. Klick auf "Stapel herunterladen" am unteren Ende der Stapelübersicht.

2. Wenn du einen Stapel gefunden hast, der dich interessiert, klick auf "Download", um das Stapelpaket
   herunterzuladen

3. Doppelklicke auf die heruntergeladene Datei oder geh auf *Datei* > *Importieren*,
   um den Stapel in Anki zu laden.

Beachte bitte, dass es derzeit nicht möglich ist, öffentliche Stapel direkt zu
deinem AnkiWeb-Konto hinzuzufügen. Du musst sie mit dem Desktop-Programm
importieren und dann [synchronisieren](syncing.md), um sie auf AnkiWeb hochzuladen.

Einen eigenen Stapel zu erstellen, ist die effektivste Möglichkeit, ein komplexes
Thema zu lernen. Themen wie Sprachen oder Naturwissenschaften können nicht einfach
durch Auswendiglernen begriffen werden. Sie benötigen Erklärungen und Kontext,
um sie effektiv zu lernen. Außerdem zwingt dich das eigenhändige Eingeben der
Informationen zu entscheiden, was die wesentlichen Aspekte sind, was widerum zu
einem besseren Verständnis führt.

Wenn du eine Sprache lernst, ist es verlockend, eine lange List von Vokabeln und
ihren Übersetzungen herunterzuladen, aber das wird dir genausowenig eine Sprache
beibringen, wie dich das Auswendiglernen von wissenschaftlichen Gleichungen
Astrophysik lehrt. Um wirklich zu lernen brauchst du Lehrbücher, Lehrer oder
Zugang zu Sätzen aus der echten Welt.

    Lerne nicht, was du nicht verstehst.
    — SuperMemo

Die meisten öffentlichen Stapel werden von Leuten erstellt, die Stoff außerhalb
von Anki lernen — aus Lehrbüchern, Kursen, dem Fernsehen, etc. Sie wählen die
interessanten Punkte von dem, was sie lernen, aus und geben sie in Anki ein.
Sie bemühen sich nicht, Hintergrundinformationen oder Erklärungen zu den Karten
hinzuzufügen, da sie den Stoff ohnehin schon verstehen. Wenn dann jemand ihren
Stapel herunterlädt und versucht, ihn zu benutzen, wird ihm das große Schwierigkeiten
bereiten, weil ihm die Hintergrundinformationen oder Erklärungen fehlen.

Das soll nicht bedeuten, dass öffentliche Stapel nutzlos sind — nur, dass sie
bei komplexen Themen als Ergänzung und nicht als Ersatz für externes Material
verwendet werden sollten.
Wenn du mit einem bestimmten Lehrbuch lernst und jemand einen Stapel mit Ideen
aus diesem Buch geteilt hat, ist das eine gute Möglichkeit, etwas Zeit zu sparen.
Auch für einfache Themen, die praktisch nur aus einer Liste von Fakten bestehen,
zum Beispiel Hauptstädte oder Trivialwissen, brauchst du vermutlich kein Material
aus externen Quellen. Aber wenn du versuchst, ein komplexes Thema ohne externes
Material zu lernen, wirst du vom Ergebnis wahrscheinlich enttäuscht sein.
