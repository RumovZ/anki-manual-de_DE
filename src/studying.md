# Lernen

<!-- toc -->

Wenn du einen Stapel gefunden hast, der dir gefällt, oder ein paar Notizen
erstellt hast, ist es an der Zeit, mit dem Lernen zu beginnen.

## Stapel

In Anki lernst du immer nur den gerade ausgewählten Stapel und dessen Unterstapel.

In der Stapelansicht werden deine Stapel mit drei Spalten aufgelistet: "Neu"
gibt die Anzahl neuer Karten an, die heute gelernt werden können. Die zweite
Spalte zeigt die Anzahl der Karten, die sich gerade in der Lernphase befinden.
"Fällig" ist die Zahl anstehender Wiederholungen.

Wenn du einen Stapel anklickst, wird er zum _aktuellen Stapel_ und Anki wechselt
in die Lernansicht. Um den aktuellen Stapel zu wechseln, kannst du jederzeit zur
Stapelansicht zurückkehren, indem du auf die entsprechende Schaltfläche am oberen
Rand des Hauptfensters klickst. Dort kannst du auch den Menüpunkt "Stapel lernen"
benutzen, um einen neuen Stapel per Tastatur auszuwählen, oder du kannst
<kbd>S</kbd> drücken, um den aktuellen Stapel zu lernen.

Du kannst das Zahnradsymbol rechts neben einem Stapel anklicken, um den Stapel
umzubenennen, zu löschen, seine Einstellungen zu bearbeiten oder ihn zu exportieren.

## Stapelübersicht

Nachdem du in der Stapelansicht auf einen Stapel geklickt hast, wird dir die
sogenannte _Stapelübersicht_ angezeigt. Dort kannst du sehen, wie viele Karten
heute fällig sind. Die Karten sind dabei in drei Kategorien aufgeteilt:

- _Neu_ bezieht sich auf Karten, die du heruntergeladen oder selbst angelegt,
  aber noch nie gelernt hast.

- _Lernen_ bezieht sich auf Karten, die du schon mal gesehen hast, aber immer
  noch lernst.

- _Wiederholen_ bezieht sich auf Karten, die du bereits gelernt hast und die
  nun wiederholt werden müssen, damit du sie nicht wieder vergisst.

Klick auf "Jetzt lernen", um zu beginnen. Anki wird dir solange Karten zeigen, bis
es keine heute fälligen mehr gibt.

Während des Lernens kannst du mit der Taste <kbd>S</kbd> zur Übersicht zurückkehren.

## Fragen

Für jede Karte wird zuerst nur die Frage gezeigt. Klick auf "Antwort zeigen"
oder betätige die <kbd>Leertaste</kbd>, nachdem du über die Antwort nachgedacht
hast. Es ist nicht schlimm, wenn du eine Weile brauchst, bis dir die Antwort
einfällt, aber als Faustregel solltest du besser aufgeben, wenn sie dir nach
etwa 10 Sekunden noch nicht eingefallen ist, anstatt dich weiter zu versuchen
zu erinnern.

Wenn die Antwort gezeigt wird, solltest du sie mit der, an die du gedacht hast,
vergleichen und Anki mitteilen, wie gut du dich erinnern konntest. Wenn du dir
nicht zutraust, deine Antwort korrekt abzugleichen, kannst du Anki dich nach
der [Eingabe deiner Antwort](templates/fields.md#checking-your-answer) fragen
lassen, anstatt dir nur Frage und Antwort zu zeigen.

## Karten (erneut) lernen

Wenn du Karten lernst oder erneut lernst, nachdem du sie vergessen hattest, zeigt
Anki sie dir mehrmals, um dir zu helfen, sie im Gedächtnis zu behalten.
Diese Abfragen heißen _Lernstufen_. Standardmäßig gibt es zwei: 1 Minute und 10
Minuten. Du kannst die Anzahl und Abstände der Stufen in den
[Stapeleinstellungen](deck-options.md#new-cards) ändern.

Beim Lernen gibt es vier Bewertungsschaltflächen:

1. _Nochmal_ schickt die Karte zurück zur ersten Lernstufe.

2. _Schwierig_ lässt die Karte die aktuelle Lernstufe wiederholen, außer es handelt
   sich um die erst Lernstufe, in welchem Fall das neue Intervall der Durchschnitt
   von _Nochmal_ und _Gut_ ist.

3. _Gut_ schickt die Karte zur nächsten [Lernstufe](deck-options.md#learning-steps).
   Wenn sich die Karte auf der letzten Lernstufe befand, wird sie in eine
   Wiederholungskarte umgewandelt, sie _steigt auf_. Standardmäßig wird eine
   aufgestiegene Karte am nächsten Tag und dann in größer werdenden Abständen wieder
   gezeigt (siehe den nächsten Abschnitt).

4. _Einfach_ wandelt die Karte sofort in eine Wiederholungskarte um, auch wenn
   noch Lernstufen übrig sind. [Standardmäßig](deck-options.md#easy-interval) wird
   die Karte nach 4 Tagen und dann in größer werdenden Abständen wieder
   gezeigt. Mit dem Zeitplaner V1 ist die _Einfach_-Schaltfläche beim erneuten Lernen
   von Karten nicht sichtbar, da sie das gleiche Intervall wie _Gut_ liefern würde.
   Mit dem [Zeitplaner V2+](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)
   erhöht sie das Intervall beim erneuten Lernen um einen zusätzlichen Tag.

Erstmalig gezeigte Karten beginnen auf der ersten Lernstufe. Wenn du also eine
Karte beim ersten Mal, das du sie siehst, mit _Gut_ bewertest, wird sie nach
10 Minuten ein weiteres Mal gezeigt und die erste Lernstufe von einer Minute wird
übersprungen.

Du kannst die Tasten <kbd>1</kbd>, <kbd>2</kbd>, <kbd>3</kbd> und <kbd>4</kbd>
benutzen, um die entsprechende Schaltfläche auszuwählen. Die <kbd>Leertaste</kbd>
und <kbd>Enter</kbd> stehen ebenfalls für _Gut_.

Wenn keine anderen Karten anstehen, zeigt Anki dir Lernkarten selbst dann, wenn
ihr Intervall noch nicht vollständig abgelaufen ist. Falls du das Intervall
lieber zur Gänze abwarten möchtest, kannst du dieses Verhalten unter
_[Einstellungen](preferences.md) > Neu planen > Grenzwert für vorgezogenes Lernen_
anpassen.

## Karten wiederholen

Wenn eine Karte zuvor gelernt wurde und zur Wiederholung ansteht, gibt es vier
Bewertungsschaltflächen:

1. _Nochmal_ kennzeichnet deine Antwort als falsch und weist Anki an, dir die
   Karte in Zukunft öfter zu zeigen. Die Wiederholung wird als _Fehlschlag_
   bezeichnet. Siehe den Abschnitt [Fehlschläge](deck-options.md#lapses) für
   Informationen darüber, wie mit gescheiterten Wiederholungen verfahren wird.

2. _Schwierig_ zeigt die Karte standardmäßig nach einem
   [etwas längeren Zeitraum](deck-options.md#hard-interval) wieder und weist Anki
   an, dir die Karte in Zukunft öfter zu zeigen.

3. _Good_ teilt Anki mit, dass das letzte Intervall in etwa angemessen war und
   die Leichtigkeit der Karte nicht nach oben oder unten angepasst werden muss.
   Mit der [voreingestellten Leichtigkeit](deck-options.md#starting-ease) ist der
   Zeitraum bis zur nächsten Wiederholung ungefähr der zweieinhalb-fache des letzten
   Zeitraums. Wenn du also zuletzt 10 Tage gewartet hast, bis die Karte gezeigt
   wurde, werden es nun 25 Tage sein.

4. _Einfach_ teilt Anki mit, dass der Zeitraum zu kurz war. Die Karte wird für
   einen [späteren Zeitpunkt als mit _Gut_](deck-options.md#easy-bonus) geplant
   und seltener gezeigt werden. Da _Einfach_ das Intervall rapide ansteigen lässt,
   sollte es nur für die allereinfachsten Karten benutzt werden. Üblicherweise
   solltest du stattdessen mit _Gut_ bewerten.

Wie schon bei Lernkarten kannst du die Tasten <kbd>1</kbd>, <kbd>2</kbd>,
<kbd>3</kbd> und <kbd>4</kbd> zur Bewertung nutzen. <kbd>Leertaste</kbd> und
<kbd>Enter</kbd> bewerten mit _Gut_.

Siehe [Stapeleinstellungen](deck-options.md) und die
[FAQs](https://faqs.ankiweb.net/what-spaced-repetition-algorithm.html), um mehr
über die Funktionsweise des Algorithmus zu lernen.

## Anzahl fälliger Karten

Während nur die Frage zu sehen ist, zeigt Anki drei Zahlen am unteren Ende des
Bildschirms an, z.B. `12 + 34 + 56`. Sie stehen für neue Karten, Karten in der
Lernphase und zu wiederholende Karten. Wenn du sie lieber nicht sehen würdest,
kannst du sie in Ankis [Einstellungen](preferences.md) abschalten.

Mit dem V1-Zeitplaner zählen die _Wiederholungen_, die nötig sind, bis alle
anstehenden Karten abgearbeitet sind, nicht die Anzahl der _Karten_. Wenn du
mehrere Lernstufen für fehlgeschlagene Wiederholungen eingestellt hast, steigt
die Zahl bei einem Fehlschlag um mehr als 1, da die Karte nun mehrfach gezeigt
werden muss.

Ab dem V2-Zeitplaner zählen _Karten_, sodass die Anzahl immer um 1 steigt, egal
wie viele Lernstufen verbleiben.

Sobald die Antwort sichtbar ist, zeigt Anki über jeder Schaltfläche eine
Schätzung davon, wann die Karte das nächste Mal gezeigt werden wird.
Wenn du das lieber nicht sehen würdest, kannst du es in Ankis
[Einstellungen](preferences.md) abschalten.

## Zufallsfaktor

Wenn du eine Wiederholungskarte bewertest, wendet Anki zudem einen geringen
Zufallsfaktor ("_Fuzz_") an, um zu vermeiden, dass Karten, die gleichzeitig
eingeführt wurden, zusammebleiben und auch in Zukunft stets am selben Tag
angezeigt werden.
Seit dem V3-Zeitplaner wird dieser Zufallsfaktor auf den Schaltflächenbeschriftungen
berücksichtigt. Wenn du also einen der vorherigen Zeitplaner benutzt und eine
geringe Abweichung zwischen den Bewertungsschaltflächen und den tatsächlichen
Intervallen feststellst, ist das vermutlich die Ursache.

Lernkarten werden ebenfalls mit bis zu 5 Minuten Verzögerung angezeigt, damit
sie nicht immer in derselben Reihenfolge erscheinen, allerdings wird das von den
Bewertungsschaltflächen nicht berücksichtigt. Diese Funktion kann nicht abgeschaltet
werden.

## Bearbeiten und Sonstiges

Du kannst auf die Schaltfläche **Bearbeiten** in der linken unteren Ecke klicken,
um die aktuelle Notiz zu bearbeiten. Anschließend kannst du weiterlernen.
Das Bearbeiten-Fenster funktioniert ganz ähnlich wie das [Hinzufügen-Fenster](editing.md).

In der rechten unteren Ecke des Wiederholungsfenster befindet sich die Schaltfläche
**Mehr**. Sie bietet einige weitere Funktionen für die aktuelle Karte oder Notiz:

- [**Markieren**](editing.md#using-flags): Fügt der Karte eine farbige Markierung
  hinzu oder entfernt sie wieder. Diese Markierungen sind beim Lernen sichtbar und
  können zur Suche in der Kartenverwaltung verwendet werden. Das ist nützlich,
  wenn du mit der Karte zu einem späteren Zeitpunkt noch etwas machen möchtest,
  z.B. ein Wort nachschlagen, sobald du zuhause bist.
  Ab Anki 2.1.45+ kannst du den Markierungen von der [Kartenverwaltung](browsing.md)
  aus Namen geben.

- **Karte / Notiz zurückstellen**: Verbirgt die Karte bzw. alle Karten der Notiz bis
  zum nächsten Tag. (Wenn du Karten schon früher wieder sehen möchtest, kannst du
  auf die Schaltfläche _Zurückstellen aufheben_ in der
  [Stapelübersicht](studying.md#study-overview) klicken.)
  Das ist nützlich, wenn du die Karte gerade nicht beantworten kannst oder später
  auf sie zurückkommen möchtest. Eine Zurückstellung kann auch
  [automatisch](studying.md#siblings-and-burying) für Karten derselben Notiz erfolgen.

  Mit dem alten Zeitplaner wurden zurückgestellte Lernkarten wieder als neue
  oder Wiederholungskarten eingereiht.

  Mit dem [Zeitplaner 2.1](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)
  werden die Lernstufen durch eine Zurückstellung hingegen nicht zurückgesetzt.

- **Fälligkeitsdatum auswählen**: Reiht die Karte in die Wiederholungsschlange ein und
  lässt sie [zu einem bestimmten Datum fällig](browsing.md#cards) werden.

- **Karte / Notiz aussetzen**: Verbirgt die Karte bzw. alle Karten der Notiz bis
  sie manuell wieder eingesetzt wird ("wieder einsetzen" in der Kartenverwaltung).
  Das ist nützlich, wenn du die Karte erstmal nicht wiederholen, aber auch nicht
  löschen möchtest.
  Mit dem alten Zeitplaner wurden ausgesetzte Lernkarten wieder als neue
  oder Wiederholungskarten eingereiht.

  Mit dem [Zeitplaner 2.1](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)
  werden die Lernstufen durch eine Aussetzung hingegen nicht zurückgesetzt.

- **Optionen**: Erlaubt die Bearbeitung der [Optionen](deck-options.md) des aktuellen
  Stapels.

- **Karteninformation**: Zeigt [statistische Daten](stats.md#card-info) zur Karte.

- [**Notiz kennzeichnen**](editing.md#the-marked-tag): Fügt der Notiz das Schlagwort
  _marked_ ("markiert") hinzu, sodass sie leicht in der Kartenverwaltung
  wiedergefunden werden kann. Das ist ähnlich, wie einzelnen Karten Flaggen zuzuweisen,
  aber da es sich hier um ein Schlagwort handelt, werden bei einer Suche danach
  alle Karten einer Notiz angezeigt. Für die meisten Benutzer sind Flaggen angemessener.

- **Notiz löschen**: Löscht die Notiz und all ihre Karten.

- **Erneut abspielen**: Spielt eventuell vorhandene Audiodateien auf der Vor- oder
  Rückseite erneut ab.

- **Audio anhalten**: Hält eine eventuell abspielende Audiodatei an.

- **Audio -5s / +5s**: Springt in der abspielenden Audiodatei 5 Sekunden zurück bzw. vor.

- **Eigene Stimme aufzeichnen**: Zeichnet den Ton deines Mikrofons auf, damit du
  deine Aussprache prüfen kannst. Diese Aufnahme is temporär und verschwindet,
  sobald du zur nächsten Karte übergehst. Wenn du einer Karte dauerhaft Ton
  hinzufügen willst, kannst du das im Bearbeiten-Fenster machen.

- **Aufnahme abspielen**: Spielt deine Aufnahme erneut ab. (Für gewöhnlich nach
  Zeigen der Antwort.)

## Anzeigereihenfolge

Beim Lernen werden Karten des ausgewählten Stapels und aller enthaltenen Stapel
angezeigt. Wenn du also den Stapel "Französisch" auswählst, werden auch die
Stapel "Französisch::Vokabeln" und "Französisch::Mein Lehrbuch::Lektion 1" angezeigt.

Wie Anki Karten aus den Stapeln entnimmt, hängt vom verwendeten Algorithmus ab:

- Mit dem V1-Zeitplaner erscheinen die Karten
  [der Reihe nach aus jedem Stapel](studying.md#display-order).

- Mit dem [V2-Zeitplaner](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html)
  werden aus allen Unterstapeln gleichzeitig Karten entnommen. Die Wiederholungsgrenzwerte
  der Unterstapel werden ignoriert - nur der des ausgewählten Stapels wird
  berücksichtigt.

- Mit dem [V3-Zeitplaner](https://faqs.ankiweb.net/the-2021-scheduler.html)
  werden die Grenzwerte der Unterstapel ebenfalls berücksichtigt und die Karten
  müssen auch nicht in der Reihenfolge der Stapel angezeigt werden.
  Siehe das Kapitel [Stapeloptionen](deck-options.md#review-sort-order) für
  weitere Informationen.

Standardmäßig entnimmt Anki neue Karten aus den Stapeln in alphabetischer Reihenfolge.
Im obigen Beispiel würdest du also erst die Karten von "Französisch", dann die von
"Französisch::Mein Lehrbuch" und schließlich die von "Französisch::Vokabeln" sehen.
Das kannst du dir zunutze machen, um die Anzeigereihenfolge der Karten zu kontrollieren,
indem du wichtige Karten in Stapeln ganz oben auf der Liste platzierst.
Wenn Computer Text sortieren, kommt das Symbol "`-`" vor allen Buchstaben des
Alphabets und das Symbol "`~`" danach. Du könntest den Stapel also "-Vokabeln"
nennen, damit er zuerst erscheint, und den anderen Stapel "\~Mein Lehrbuch",
damit er als allerletztes erscheint.

Neue und Wiederholungskarten werden unabhängig entnommen und Anki wartet nicht,
bis beides erschöpft ist, bevor es zum nächsten Stapel übergeht. Es kann also
passieren, dass du neue Karten von einem Stapel und Wiederholungskarten von einem
anderen siehst, oder umgekehrt. Wenn du das vermeiden willst, solltest du anstelle
des Oberstapels direkt den Stapel, den du lernen möchtest, auswählen.

Da Lernkarten in gewisser Weise zeitkritisch sind, werden sie aus allen Stapeln
gleichzeitig entnommen und in der Reihenfolge ihrer Fälligkeit angezeigt.

Um die Anzeigereihenfolge eines bestimmten Stapels zu beeinflussen oder neue
Karten in zufälliger Reihenfolge erscheinen zu lassen, siehe bitte die
[Stapeloptionen](deck-options.md). Für eine präzisere Anordnung neuer Karten kannst
du ihre Reihenfolge in der [Kartenverwaltung](browsing.md) festlegen.

## Geschwister und Zurückstellen

Im Kapitel [Grundlagen](getting-started.md) haben wir gesehen, dass Anki für jeden
Eingabenblock mehr als eine Karte erzeugen kann, z.B. eine Karte Vorderseite→Rückseite
und eine Rückseite→Vorderseite oder zwei Lückentexte zum selben Text.
Diese zusammengehörigen Karten heißen _Geschwister_.

Wenn du eine Karte mit Geschwistern beantwortest, kann Anki verhindern, dass diese
Geschwister in derselben Lerneinheit gezeigt werden, in dem es sie automatisch
zurückstellt. Zurückgestellte Karten sind von der Wiederholung ausgenommen, bis
ein neuer Tag beginnt oder du sie mit der Option "Zurückstellen aufheben" am unteren
Ende der Stapelübersicht zurückholst.
Anki stellt sogar Geschwister zurück, die nicht im selben Stapel sind (z.B. weil
du die Funktion [_Stapel überschreiben_](templates/intro.md) benutzt).

Du kannst das Zurückstellen von den [Stapeloptionen](deck-options.md) aus aktivieren.
Es gibt getrennte Einstellungen für neue und Wiederholungskarten.

Anki stellt nur neue und Wiederholungskarten zurück. Lernkarten sind nicht betroffen,
da der zeitliche Abstand für sie entscheidend ist. Wenn du andererseits eine
Lernkarte beantwortest, werden ihre Geschwister, die neue oder Wiederholungskarten
sind, zurückgestellt.

Anmerkung: Eine Karte kann nicht zugleich ausgesetzt und zurückgestellt sein.
Das Aussetzen einer Karte hebt ihre Zurückstellung auf. Ausgesetzte Karten
können in Anki 2.1.49+ nicht zurückgestellt werden, wohingegen es in früheren Versionen
die Aussetzung aufhebt.

## Tastenkombinationen

Die meisten gebräuchlichen Funktionen in Anki haben Tastenkombinationen, die über
die Benutzeroberfläche in Erfahrung gebracht werden können: Menüpunkte führen ihre
Tastenkombinationen rechts neben sich auf und Schaltflächen offenbaren sie meistens,
wenn die Maus über sie bewegt wird.

Beim Lernen zeigen <kbd>Leertaste</kbd> oder <kbd>Enter</kbd> die Antwort.
Anschließend können die Tasten <kbd>1</kbd> bis <kbd>4</kbd> benutzt werden,
um eine bestimmte Bewertung zu wählen. Viele Benutzer finden es praktisch, die
meisten Karten mit <kbd>Leertaste</kbd> zu bewerten und einen Finger auf <kbd>1</kbd>
zu halten, für den Fall, dass sie eine Karte vergessen.

Die Funktion _Stapel lernen_ im Werkzeugmenü erlaubt es, schnell mit der Tastatur
den Stapel zu wechseln. Du kannst sie mit der Taste <kbd>/</kbd> auslösen.
Es werden alle deine Stapel und oben ein Filterbereich angezeigt. Während du tippst,
begrenzt Anki die Anzeige auf passende Stapel. Mit einem Leerzeichen kannst
du mehrere Suchbegriffen angeben, die alle zutreffen müssen.
Zu "ja 1" und "on1 ja" würde beidem ein Stapel namens "Japanisch::Lektion1" passen.

## Rückstände

Wenn du mit deinen Wiederholungen in Verzug gerätst, priorisiert Anki die Karten,
die schon am längsten gewartet haben, und zeigt sie in zufälliger Reihenfolge,
bis dein täglicher Wiederholungsgrenzwert erreicht ist. Das garantiert, dass keine
Karte für immer wartet, bedeutet aber auch, dass neue Karten, die du einführst,
nicht wiederholt werden, bis du deinen Rückstand aufgeholt hast.

Wenn du die Anzeigereihenfolge der überfälligen Wiederholungen ändern möchtest,
kannst du zu diesem Zweck einen [Auswahlstapel](filtered-decks.md) erstellen.

Wenn du überfällige Karten beantwortest, bezieht Anki die zusätzlich verstrichene
Zeit bei der Berechnung, wann die Karte das nächste Mal gezeigt werden soll, mit
ein. Siehe bitte den Abschnitt über Ankis
[_Spaced-Repetition_-Algorithmus](https://faqs.ankiweb.net/due-times-after-a-break.html)
für weitere Informationen.
