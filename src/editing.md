# Hinzufügen/Bearbeiten

<!-- toc -->

## Notizen und Karten hinzufügen

In den [Grundlagen](getting-started.md) haben wir besprochen, dass man in Anki
nicht direkt Karten, sondern Notizen hinzufügt und Anki die Erstellung der Karten übernimmt.
Du kannst das "Hinzufügen"-Fenster mit einem Klick auf die entsprechende Schaltfläche
in der Hauptansicht öffnen.

In der linken oberen Ecke dieses Fensters wird der aktuelle Notiztyp angezeigt.
Sollte dort nicht "Einfach" stehen, hast du vermutlich Notiztypen
durch Herunterladen eines geteilten Stapels hinzugefügt. Im Folgenden gehen wir davon aus,
dass der Notiztyp "Einfach" ausgewählt ist.

In der rechten oberen Ecke steht der Name des Stapels, in dem die neuen Karten landen werden.
Wenn du einen neuen Stapel für deine Karten erstellen willst, klicke auf den aktuell ausgewählten
Stapel und wähle im Folgefenster "Hinzufügen".

Unterhalb dieser Schaltflächen befinden sich einige Werkzeuge sowie zwei Eingabeflächen,
die mit "Vorderseite" und "Rückseite" beschrieben sind. Diese Eingabeflächen werden
"Felder" genannt. Felder können durch einen Klick auf die Schaltfläche "Felder…" hinzugefügt,
entfernt oder umbenannt werden.

Unterhalb der Felder gibt es einen weiteren Bereich für "Schlagwörter".
Schlagwörter sind wie Etiketten, die du an deine Notizen anhängen kannst, um deine Sammlung
zu strukturieren und Notizen einfacher zu finden. Du kannst mehrere Schlagwörter hinzufügen,
indem du sie mit Leerzeichen voneinander trennst. So würde z. B. die Eingabe

    Vokabeln mit_Tutor_durchgehen

… zwei Schlagwörter an die Notiz anhängen.
Du kannst diesen Bereich aber auch leer lassen.

Hast du Text auf Vorder- und Rückseite eingegeben, kannst du die Notiz mit einem
Klick auf die Schalfläche "Hinzufügen" oder mit dem Tastaturkürzel <kbd>Strg</kbd>
+<kbd>Enter</kbd> (<kbd>⌘</kbd>+<kbd>Enter</kbd> auf dem Mac) zu deiner Sammlung hinzufügen.
Zusätzlich wird eine Karte erstellt und in den aktuell ausgewählten Stapel einsortiert.
Du kannst auch nach der Erstellung noch Änderungen an deinen Notizen vornehmen.
Klicke auf die Schaltfläche "Verlauf", um in der [Kartenverwaltung](browsing.md)
nach einer kürzlich hinzugefügten Notiz zu suchen.

Für eine Erklärung der Werkzeuge, die sich im Bereich zwischen Notiztyp und Feldern befinden,
siehe den Abschnitt [Funktionen des Editors](#funktionen-des-editors).

### Duplikatüberprüfung

Anki überprüft das erste Feld auf Einzigartigkeit. Erstellst du z. B. eine Notiz mit
der Vorderseite "Apfel", obwohl sich bereits eine derartige Notiz in deiner Sammlung befindet,
wird Anki dich mit einer Warnung darauf hinweisen.
Die Duplikatüberprüfung ist jedoch auf den aktuellen Notiztyp beschränkt. Anki wird also keine
Warnung anzeigen, wenn das Wort "Apfel" auf der Vorderseite mehrerer Notizen von unterschiedlichen
Notiztypen steht (z. B. ein Notiztyp für Japanisch und einer für Französisch).

Aus Effizienzgründen überprüft Anki die restlichen Felder nicht automatisch auf Duplikate.
Die Kartenverwaltung bietet jedoch eine Funktion namens "Duplikate suchen", die du bei Bedarf
manuell ausführen kannst.

###  Effektiv lernen

Jeder hat seine eigenen Vorlieben, wenn es um die Wiederholung von Lernstoff geht.
Es gibt jedoch eine Reihe allgemeingültiger Konzepte, die man stets im Hinterkopf behalten
sollte. [Dieser Artikel](http://supermemo.org/deutsch/articles/20rules.htm) von SuperMemo
bietet eine hervorragende Einführung, insbesondere die folgenden Punkte:

- **Halte es einfach**: Je kürzer deine Karten sind, desto einfacher wird es sein,
  sie zu wiederholen. Du magst vielleicht in Versuchung kommen, möglichst viele Fakten
  "sicherheitshalber" mitaufzunehmen - die Wiederholungen würden aber durch das Übermaß
  an Information schnell zur Belastung werden.

- **Lerne nicht auswendig, was du nicht verstehst**: Versuche, lange Vokabellisten beim
  Erlernen einer Sprache zu vermeiden. Neue Sprachen lernt man am besten
  kontextuell. Das bedeutet, Wörter so zu lernen, wie sie in
  Wirklichkeit verwendet werden: in ganzen Sätzen. Das gilt auch für alle anderen
  Disziplinen. Stell dir vor, du machst einen Computer-Kurs und möchtest dir eine
  große Menge an Abkürzungen merken. Ohne Kontext wird dir das vermutlich schwer fallen.
  Wenn du dir aber die Zeit nimmst, um die Konzepte hinter den Abkürzungen zu
  verstehen, wird das Auswendiglernen wesentlich leichter von der Hand gehen.

## Notiztypen hinzufügen

Die Standardnotiztypen sind gut geeignet für simple Karten mit nur einem Wort oder Satz
je Seite. Sobald du jedoch mehr als eine Information in
einer Notiz unterbringen willst, solltest du den Inhalt auf mehrere Felder
verteilen.

Vielleicht denkst du: "Aber ich will nur eine Karte,
warum kann ich nicht einfach eine Audiodatei, ein Bild, einen Hinweis
und die Übersetzung in das Feld *Vorderseite* eingeben?"
Wenn du das bevorzugst, geht das natürlich in Ordnung. Diese Herangehensweise hat
jedoch einen großen Nachteil: All diese Informationen sind untrennbar miteinander verbunden.
So bist du dann z. B. nicht in der Lage, die Karten nach dem Hinweis zu sortieren, da dieser
mit dem restlichen Inhalt vermischt ist.
Die Aufteilung des Inhalts auf mehrere Felder erleichtert eine spätere Bearbeitung
deiner Karten deutlich. Würdest du im oben genannten Beispiel die Audiodatei
von der Vorder- auf die Rückseite bringen wollen, müsstest du das manuell für
jede einzelne Notiz erledigen. Hast du jedoch ein eigenes Feld für die Audiodatei,
musst du nur einmal die Kartenvorlage anpassen, um alle Notizen zu ändern.

Um einen neuen **Notiztyp** zu erstellen, wähle den Eintrag
`Werkzeuge → Notiztypen verwalten` in der Hauptansicht von Anki und klicke auf "Hinzufügen".
Es öffnet sich ein neues Fenster, das eine Auswahl an Notiztypen
anbietet, auf denen der neue Notiztyp basieren soll.
"Hinzufügen" bedeutet also, einen Notiztyp nach einer von Anki's Vorlagen zu erstellen.
Soll der neue Notiztyp auf einem Notitzyp aus deiner Sammlung basieren,
wähle stattdessen "Klonen" aus. Hast du z. B. bereits einen Notiztyp für
Französischvokabeln, könntest du einen Klon für Spanischvokabeln erstellen.

Nach dem Klick auf OK wird dich Anki nach einem Namen für den neuen Notiztyp fragen.
Das Fach des Lernmaterials ist zumeist eine gute Wahl, z. B. "Japanisch",
"Allgemeinwissen" etc. Nach Eingabe des Namens kannst du den Dialog schließen
und zum Editor zurückkehren.

## Felder anpassen

Um die Felder eines Notiztyps anzupassen, klicke bei der Erstellung
oder Bearbeitung von Notizen im Editor, oder nach Auswahl des Notiztyps
im Fenster "Notiztypen verwalten" auf die Schaltfläche "Felder…".

Du kannst mit den entsprechenden Schaltflächen Felder hinzufügen,
entfernen oder umbenennen. Im Dialog "Position ändern" kannst du die numerische
Position eines Feldes im Editor festlegen. Willst du, dass ein bestimmtes
Feld an erster Stelle erscheint, ändere dessen Position auf "1".

"Tags", "Type", "Deck", "Card" und "FrontSide" sind spezielle, von Anki
[reservierte Feldnamen](templates/fields.md#special-fields) und sollten
deshalb nicht verwendet werden.

Mithilfe der Bedienelemente auf der unteren Hälfte des Fensters kannst du
verschiedene Eigenschaften der Felder im Editor festlegen.
Wichtig: In diesem Fenster wird _nicht_ festgelegt, wie der Inhalt deiner Felder
beim Wiederholen auf deinen Karten aussieht.
Das ist die Aufgabe der [Vorlagen](templates/intro.md).

**Schriftart festlegen** \
Damit lässt sich die Schriftart und Größe ändern, in welcher der Textinhalt
des jeweiligen Feldes angezeigt wird. Das kann beispielsweise nützlich sein,
wenn du unwichtige Informationen kleiner darstellen oder die Größe fremder
Schriftzeichen erhöhen willst, um sie lesbarer zu machen.
Nochmals: Diese Einstellungen haben keine Auswirkungen auf das Aussehen
der Karten im Rahmen der Wiederholung.
Das Design wird mittels CSS in den [Vorlagen](templates/intro.md) festgelegt.
Notiztypen mit der Funktion "Antwort eintippen" stellen hier eine Ausnahme dar:
Der einzugebende Text verwendet die Schriftgröße, die du hier
definierst.
(Wie du bei solchen Notiztypen die Schriftart für das Eingabefeld ändern kannst,
erfährst du im Abschnitt [Antwort überprüfen](templates/fields.md#checking-your-answer)).

**In der Kartenverwaltung nach diesem Feld sortieren** \
Mit dieser Einstellung kannst du das Feld festlegen, das für die Spalte
"Sortierfeld" in der Kartenverwaltung verwendet werden soll. So lassen sich
Notizen und Karten alphabetisch nach dem Feldinhalt ordnen.
Ein Notiztyp kann jeweils nur ein Sortierfeld haben.

**Textrichtung umkehren** \
Verwende diese Funktion für Sprachen, deren Leserichtung von rechts nach links
verläuft (engl. _"right to left"_ = "RTL"), z. B. Arabisch oder Hebräisch.
Auch hier gilt: Diese Einstellung betrifft lediglich die Anzeige des
Feldinhalts im Editor. Für die korrekte Darstellung des Textes sind
[weitere Anpassungen der Vorlage](templates/styling.md#text-direction) notwendig.

Nachdem du neue Felder hinzugefügt hast, wirst du sie wahrscheinlich auch
zur Vorder- oder Rückseite deiner Karten hinzufügen wollen. Wie das funktioniert,
lernst du im Kapitel [Vorlagen](templates/intro.md).

## Stapel oder Notiztyp ändern

Während du Notizen hinzufügst, kannst du mit der Schaltfläche "Typ" (links oben)
den Notiztyp ändern, der für die nächste Notiz verwendet werden soll. Analog funktioniert
die Schaltfläche "Stapel" (rechts oben) für die Festlegung des Zielstapels.
Das jeweilige Fenster erlaubt nicht nur die Auswahl existierender Stapel oder Notiztypen,
sondern auch das Hinzufügen neuer Stapel/Notiztypen und die Verwaltung bestehender Notiztypen.

## Material strukturieren

### Stapel richtig verwenden

[Stapel](getting-started.md#stapel) haben den Zweck, Material in breite
Kategorien aufzuteilen, die du unabhängig voneinander lernen willst, z. B.
Englisch, Geographie usw. Es mag verlockend erscheinen, eine Menge kleiner
Stapel zu erstellen, um deinem Lernmaterial Struktur zu geben, z. B.
"Mein Geographie-Lehrbuch Kapitel 1", oder "Essensverben", wir raten jedoch
aus folgenden Gründen davon ab:

- Eine große Anzahl kleiner Stapel kann bedingen, dass deine Karten in einer
  erkennbaren Reihenfolge erscheinen. Ältere Versionen des Zeitplaners
  können neue Karten nämlich nur in der Reihenfolge der Stapel einführen.
  Und falls du vorhast, jeden Stapel einzeln durchzugehen (was nebenbei bemerkt
  recht ineffizient ist), würden alle Karten aus "Kapitel 1" bzw. "Essensverben"
  gemeinsam kommen. Das vereinfacht die Beantwortung der Fragen, weil
  du die Karten aus ihrem Kontext erraten könntest, was wiederum eine Verschlechterung
  der Lernqualität bedeuten würde. In realen Testsituationen solltest du auch nicht
  darauf bauen, Denkanstöße durch verwandte Inhalte zu bekommen!

- Obwohl das Ausmaß dieses Problems in neueren Versionen etwas eingedämmt wurde,
  können sich hunderte von Stapeln negativ auf die Leistung des Programms auswirken.
  Bei Anki-Versionen unterhalb von 2.1.50 können übergroße Stapelhierarchien
  sogar zu Anzeigefehlern in der Stapelübersicht führen.

### Schlagwörter verwenden

Anstatt eine Menge kleiner Stapel zu erstellen, solltest du Schlagwörter und/oder
Felder verwenden, um dein Lernmaterial zu strukturieren.
Schlagwörter sind äußerst hilfreich, um Suchergebnisse zu verbessern,
spezifische Inhalte zu finden und deine Sammlung zu ordnen.
Es gibt eine Unzahl an Möglichkeiten, Schlagwörter und Flaggen effektiv zu nutzen,
weshalb es ratsam ist, dir bereits im Vorhinein zu überlegen, wie du sie verwenden willst.

Manche bevorzugen es, Stapel und Unterstapel zur Stukturierung zu verwenden.
Schlagwörter haben aber einen großen Vorteil: Eine Karte kann beliebig viele
Schlagwörter beinhalten, sie kann jedoch nur zu einem Stapel gehören. Das macht
Schlagwörter in den meisten Fällen zu einem wesentlich stärkeren und flexibleren
Kategorisierungssystem als Unterstapel.

Statt einen Stapel namens "Essensverben" zu erstellen, könntest du diese Karten
in deinen Hauptstapel für diese Sprache legen und ihnen die Schlagwörter "Essen"
und "Verb" geben.
Da jede Karte mehrere Schlagwörter beinhalten kann, eröffnen sich Möglichkeiten wie
die [Suche](searching.md#tags-decks-cards-and-notes) nach allen Verben, oder allen Vokabeln,
die etwas mit "Essen" zu tun haben, oder allen Verben, die zum Thema "Essen" gehören.

Du kannst Notizen sowohl im Editor des "Hinzufügen"-Fensters als auch in dem der
[Kartenverwaltung](browsing.md) Schlagwörter geben. Du kannst
auch neue Schlagwörter hinzufügen und bestehende umbenennen oder organisieren.
Bitte beachte, dass Schlagwörter auf der Notiz-Ebene gespeichert werden. Das heißt,
dass das Hinzufügen eines Schlagworts zu einer Karte automatisch auch
alle Geschwister dieser Karte betrifft. Um eine einzelne Karte ohne ihre
Geschwister zu kennzeichnen, kannst du Flaggen verwenden, da diese auf der
Karten-Ebene gespeichert werden.

### Flaggen verwenden

Flaggen funktionieren ähnlich wie Schlagwörter, werden beim Wiederholen aber
rechts oben angezeigt. Du kannst auch in der Kartenverwaltung nach Karten mit
einer bestimmten Flagge suchen, Flaggen in der Seitenleiste umbenennen und Auswahlstapel
aus Karten erstellen, die mit einer bestimmten Flagge gekennzeichnet wurden.
Im Gegensatz zu Schlagwörtern kann eine Karte nur eine Flagge auf einmal zugewiesen bekommen. 
Ein weiterer wichtiger Unterschied besteht darin, dass Flaggen auf der
[Kartenebene](getting-started.md#karten) gespeichert werden, d. h. das Zuweisen
einer Flagge zu einer Karte hat keine Auswirkungen auf deren Geschwister.

Du kannst Karten direkt beim Wiederholen eine Flagge zuweisen bzw. diese wieder entfernen,
indem du das Tastaturkürzel <kbd>Strg</kbd> + <kbd>1-7</kbd> (<kbd>⌘</kbd> + <kbd>1-7</kbd>
auf dem Mac) drückst. Das funktioniert auch in der [Kartenverwaltung](browsing.md).


### Das Schlagwort "marked"

Anki behandelt das Schlagwort "marked" (engl. für "markiert") gesondert.
Beim Wiederholen und in der Kartenverwaltung gibt es Funktionen, um
dieses Schlagwort schnell hinzuzufügen oder zu entfernen.
In der Wiederholungsansicht wird mit einem Stern in der linken oberen Ecke angezeigt,
ob die aktuelle Karte das Schlagwort "marked" enthält. Karten, deren Notiz
auf diese Weise markiert ist, werden in der Kartenverwaltung mit einer
anderen Farbe hinterlegt.

Info: Diese Funktion gibt es nur mehr aus Kompatibilitätsgründen mit älteren
Versionen. In den meisten Fällen sind Flaggen besser geeignet.


### Felder verwenden

Sollten Schlagworte nicht ausreichen, kann man auch designierte Felder zur
inhaltlichen Klassifizierung verwenden, z. B. "Buch", "Seite" o. ä.
Man kann die Suche nämlich auf bestimmte Felder einschränken. So sind sehr spezifische
Suchanfragen möglich, wie z. B. `"Buch:Grimm's Märchen" Seite:63`.

### Benutzerdefiniertes Lernen und Auswahlstapel

Die Funktionen Benutzerdefiniertes Lernen und [Auswahlstapel](filtered-decks.md)
ermöglichen dir, temporäre Stapel anhand von Suchbegriffen wie Schlagwörtern,
Flaggen, Markierungen und Feldern zu erstellen. So kannst du im täglichen
Gebrauch den Großteil deines Lernmaterials durchmischt in einem einzelnen
Stapel wiederholen, bei Bedarf aber jederzeit temporäre Stapel erstellen, falls
du einmal vollen Fokus auf ein bestimmtes Fach setzen musst, z. B. vor einer Prüfung.
Im Allgemeinen gilt die folgende Regel: Wenn du bestimmten Stoff immer getrennt vom
Rest wiederholen willst, solltest du ihn in einen normalen Stapel geben;
wenn du ihn hin und wieder separat durchgehen musst (z. B. vor einer Prüfung, oder um
einen Arbeitsrückstand aufzuholen), sind Auswahlstapel die bessere Wahl.

## Funktionen des Editors

Der Editor wird beim [Hinzufügen von Notizen](editing.md),
bei deren Bearbeitung im Rahmen der [Wiederholung](studying.md) und in der
[Kartenverwaltung](browsing.md) angezeigt.

Oben links befinden sich zwei Schaltflächen: Eine öffnet das Fenster für die
[Felder](editing.md#anpassung-der-felder), die andere die [Kartenvorlagen](templates/intro.md).

Rechts davon schließen sich die Formatierungswerkzeuge an. Fett, Kursiv und Unterstrichen
funktionieren, wie man es von anderen Textverarbeitungsprogrammen gewohnt ist.
Mit den nächsten beiden Schaltflächen kannst du Text tief- und hochstellen, was
praktisch sein kann für chemische Verbindungen wie H<sub>2</sub>0 oder einfache
mathematische Ausdrücke wie x<sup>2</sup>.

Der Radiergummi entfernt die Formatierung des aktuell markierten Textes -
einschließlich Farben, Schriftstärke und -stil, usw.

Dahinter reihen sich drei Werkzeuge, die der Erstellung von Listen sowie
Textausrichtung und -einrückung dienen, und zwei Schaltflächen, mit denen
du die Schriftfarbe ändern kannst.

Die Schaltfläche \[…\] ist nur sichtbar, wenn ein Lückentext-Notiztyp ausgewählt ist.

Du kannst mit dem Büroklammer-Werkzeug Audiodateien, Bilder und Videos von
deiner Festplatte auswählen und sie an deine Notiz anhängen.
Alternativ kannst du Medien auch in die Zwischenablage deines Computers
geben (z. B. durch einen Rechtsklick auf ein Bild im Internet und die Auswahl
von "Bild kopieren") und in einem Feld deiner Wahl einfügen.
Für nähere Informationen zu Medien, siehe das Kapitel [Medien](media.md).

Mit einem Klick auf das Mikrofon kannst du eine Audiodatei über das Mikrofon
deines Computers aufnehmen und in das aktuelle Feld einfügen.

Die Schaltfläche F<sub>x</sub> öffnet ein Menü, über welches du
[MathJax oder LaTeX](math.md) in die Notiz einfügen kannst.

Die Schaltfläche `</>` zeigt den zugrundeliegenden HTML-Code eines Feldes an.

Anki 2.1.45+ unterstützt das Anheften von Feldern direkt aus dem Editor.
Wenn du auf die Reißzwecke rechts oben in einem Feld klickst, wird Anki den
Inhalt dieses Feldes nach dem Hinzufügen einer Notiz beibehalten.
Das kann nützlich sein, wenn du oft hintereinander denselben Inhalt eingeben
musst. In älteren Anki-Versionen wurde diese Funktion vom Felder-Fenster
aus aktiviert.

Die meisten Bedienelemente können auch über Tataturkürzel aktiviert werden,
die angezeigt werden, wenn du mit der Maus darüber fährst.

Anki behält beim Einfügen von Inhalten über die Zwischenablage im Normalfall
den Großteil der Formatierung bei. Wenn du dabei jedoch die Umschalttaste
gedrückt hältst, werden die Inhalte ohne Formatierung eingefügt.
In den Einstellungen kannst du dieses Verhalten mit der Option
"Text aus der Zwischenablage ohne Formatierung einfügen" zum Standard machen.

## Lücken einfügen

In Lückentexten werden ein oder mehrere Wörter eines Satzes ausgeblendet.
Nehmen wir den folgenden Satz:

    Die Universität Wien wurde 1365 gegründet.

Machen wir "1365" zu einer Lücke, würde der Satz beim Wiederholen so aussehen:

    Die Universität Wien wurde […] gegründet.

"1365" ist auf der Vorderseite ausgeblendet und wird auf der Rückseite
aufgedeckt.

Siehe Regel 5 [hier](http://supermemo.org/deutsch/articles/20rules.htm),
um mehr über die Vorteile von Lückentexten zu erfahren.

Anki bietet einen eigenen Notiztyp, um einfach Lückentexte zu erstellen.
leicht macht. Um einen Lückentext zu erstellen, wähle zuerst den Notiztyp
"Lückentext" und gib dann einen Satz in das "Text"-Feld ein.
Markiere danach mit der Maus den Teil, den du verstecken willst, und klicke auf die
Schaltfläche \[…\].
Anki wird den Text dann mit doppelten geschweiften Klammern und einem Index markieren:

    Die Universität Wien wurde {{c1::1365}} gegründet.

Das "c1" bedeutet, dass du eine Lücke mit dem Index 1 erstellt hast.
Du kannst auch mehrere Lücken erstellen, wenn du willst. Wenn du in unserem
Beispiel "Die Universität Wien" auswählst und noch einmal auf \[…\] klickst, wird der
Satz nun so aussehen:

    Die {{c2::Universität Wien}} wurde {{c1::1365}} gegründet.

Fügst du diese Notiz hinzu, wird Anki zwei Karten erstellen. Die erste Karte zeigt:

    Die Universität Wien wurde […] gegründet.

… auf der Vorderseite und den vollständigen Satz auf der Rückseite. Die zweite Karte
wird auf der Vorderseite so aussehen:

    Die […] wurde 1365 gegründet.

Du kannst auch mehrere Lücken auf derselben Karte erstellen. Änderst du im obigen
Beispiel den Index c2 auf c1, wird nur eine Karte erstellt, auf der sowohl "Die Universität Wien"
als auch "1365" ausgeblendet sind. Wenn du beim Einfügen einer Lücke die <kbd>Alt</kbd>-Taste
(<kbd>Option</kbd> auf dem Mac) gedrückt hältst, behält Anki den aktuellen Index bei,
anstatt ihn zu erhöhen.

Lücken werden strikt um den markierten Text gesetzt, Wortgrenzen werden also nicht beachtet.
Wählst du "niversität Wien" statt "Universität Wien" aus, würde die Lücke in der
Wiederholung als `Die U[…] wurde 1365 gegründet.` erscheinen, was dir einen Hinweis gäbe.

Du kannst aber auch Tipps erstellen, die nicht im Text vorkommen. Wenn du den ursprünglichen
Text so eingibst:

    Die Universität Wien::Bildungseinrichtung wurde 1365 gegründet.

… und dann nach Auswahl von "Die Universität Wien::Bildungseinrichtung" auf \[…\] klickst,
wird Anki den Text hinter den zwei Doppelpunkten als Tipp interpretieren.
Das Resultat sieht dann so aus:

    Die {{c1::Universität Wien::Bildungseinrichtung}} wurde 1365 gegründet.

Bei der Wiederholung wird die Karte so erscheinen:

    Die [Bildungseinrichtung] wurde 1365 gegründet.

Es gibt auch die Möglichkeit, den Lückeninhalt bei der Wiederholung einzutippen.
Für nähere Informationen, siehe [Antworten eingeben](templates/fields.md#checking-your-answer).

Bitte beachte, dass die Verschachtelung von Lücken nicht unterstützt wird.
Die folgende Eingabe wäre also ungültig:

    Die {{c1::Universität {{c2::Wien}}}} wurde 1365 gegründet.

Wenn du überlappende Lückentexte brauchst, musst du ein zweites Feld erzeugen,
dieses in die [Vorlage](templates/intro.md) des Notiztyps einfügen und den Text
folgendermaßen in beide Felder kopieren:

    Feld 1: Die {{c1::Universität Wien}} wurde 1365 gegründet.

    Feld 2: Die {{c2::Universität}} Wien wurde 1365 gegründet.

Der Standardnotiztyp für Lückentexte hat ein zweites Feld namens "Extra",
dessen Inhalt nur auf der Rückseite der Karte erscheint.
Damit kannst du zusätzliche Informationen in deine Notiz einbauen.

"Lückentext"-Notiztypen werden von Anki besonders behandelt und können deswegen
nicht auf einem regulären Notiztyp basieren. Um einen solchen Notiztyp anzupassen,
musst du den Standardnotiztyp "Lückentext" klonen.
Formatierung und Stil können wie bei regulären Notiztypen angepasst werden,
es ist jedoch nicht möglich, zusätzliche Kartenvorlagen zu einem Notiztyp
hinzuzufügen, der auf dem Typ "Lückentext" basiert.

## Sonderzeichen und Akzente eingeben

Alle modernen Computer unterstützen die Eingabe fremder Symbole und Akzente
auf unterschiedliche Art und Weise. Wir empfehlen, die Tastaturbelegung der
Sprache zu verwenden, die du lernen willst.

Sprachen, die ihre eigene Schrift haben (z. B. Japanisch, Chinesisch, Russisch usw.)
haben stets auch spezifische Tastaturbelegungen.

Europäische Sprachen, die Akzente benutzen, haben oftmals auch eigene Belegungen,
können aber auch mit der deutschen Tastaturbelegung geschrieben werden.
Hierfür musst du zuerst den gewünschten Akzent und dann den Buchstaben eingeben,
der den Akzent erhalten soll - z. B. ergeben <kbd>`</kbd> und <kbd>A</kbd> das Symbol à.

<!-- deleted paragraph -->

<!-- deleted paragraph -->

Um herauszufinden, wie du fremde Tastaturbelegungen auf deinem Betriebssystem installieren
kannst, gib in Google Suchbegriffe wie "Japanische Tastaturbelegung Mac" oder
"Chinesische Tastaturbelegung Windows" ein.

Für Sprachen mit umgekehrter Leserichtung (RTL) wird es etwas komplizierter.
Diese [Website](http://dotancohen.com/howto/rtl_right_to_left.html) (Englisch)
bietet einen guten Ausgangspunkt.

Das Toolkit, auf dem Anki's Editor aufgebaut ist, hat Schwierigkeiten mit manchen
Eingabemethoden wie z. B. auf dem Mac das Gedrückthalten von Tasten, um akzentuierte
Buchstaben auszuwählen, oder die Eingabe von Schriftzeichen durch Kombination der
<kbd>Alt</kbd>-Taste und numerischer Codes auf Windows.

## Unicode-Normalisierung

Zeichen wie `à` können auf einem Computer auf unterschiedliche Arten gespeichert werden,
beispielsweise mit einem für das Symbol spezifischen Code, oder mit einem normalen `a`
und einem weiteren Code für den Akzent darüber. Das kann beim Mischen von Code
aus unterschiedlichen Quellen oder bei der Verwendung verschiedener Computer
Probleme verursachen. Wenn dein Computer Tastatureingaben in einer bestimmten
Form handhabt, der Inhalt aber auf eine andere Art gespeichert wird, so werden
Sonderzeichen bei Sucheingaben entsprechend der Art deines Computers nicht
gefunden, obwohl die visuelle Ausgabe beider Varianten dieselbe ist.

Um eine problemlose Suche zu gewährleisten, normalisiert Anki den Text in einen
Standard. Für die meisten Nutzer:innen ist dieser Vorgang unbemerkbar. Wenn du jedoch
sehr spezifisches Material wie altertümliche japanische Symbole lernst, kann der
Normalisierungsprozess sie ungewollt in ein moderneres Äquivalent umwandeln.

Willst du, dass Anki deine Buchstabencodes exakt beibehält - trotz des Risikos, dass
Sucheingaben fehlschlagen könnten - so kannst du das mit dem folgenden Befehl
in der [Debugging-Konsole](./misc.md) bewerkstelligen:

```python
mw.col.conf["normalize_note_text"] = False
```

Jeglicher Inhalt, der nach der Eingabe dieses Befehls hinzugefügt wird, bleibt von
der Normalisierung unberührt. Es sei hier noch einmal ausrücklich erwähnt, dass es
sich um einen Kompromiss für Spezialfälle handelt, der die Suche nach Inhalten
bei der Verwendung unterschiedlicher Betriebssysteme oder gemischter Quellen erschweren kann.
