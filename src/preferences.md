# Einstellungen

<!-- toc -->

Die Einstellungen finden sich im Menü _Werkzeuge_ auf Windows/Linux und im Anki-Menü auf einem Mac.

## Einfach

**Videotreiber**  
Ankis Programmbibliotheken benötogen einen Videotreiber, um Inhalte auf dem Bildschirm darstellen zu
können. Aufgrund unterschiedlicher Hardware- und Software-Konfigurationen hängt es von deinem Rechner
ab, welcher Treiber am besten funktioniert. ANGLE und OpenGL sind schneller als die Option Software,
aber funktionieren auf manchen Systemen vielleicht nicht richtig. Auf einem Mac ist OpenGL fast immer
die beste Wahl.

**Wiedergabesteuerelemente auf Karten mit Audiodateien anzeigen**  
Ob eine anklickbare Schaltfläche zum (erneuten) Abspielen beim Lernen von Karten mit Ton angezeigt
werden soll.

**Audiowiedergabe beim Antworten unterbrechen**  
Ob eine aktuelle Audioausgabe beendet werden soll, wenn eine Karte beantwortet wird.

**Bilder aus der Zwischenablage im PNG-Bildformat einfügen**  
Standardmäßig fügt Anki Bilder aus der Zwischenablage als JPG-Dateien ein, um Speicherplatz zu sparen.
Mit dieser Option kannst du stattdessen PNG-Dateien einfügen lassen. PNG-Bilder unterstützen durchsichtigen
Hintergrund und sind verlustfrei, resultieren aber meistens in sehr viel größeren Dateien.

**Text aus der Zwischenablage ohne Formatierung einfügen**  
Standardmäßig wird Formatierung wie Schriftstärke und Farbe beim Einfügen beibehalten, außer es wird
die <kbd>Umschalttaste</kbd> gedrückt. Diese Option kehrt dieses Verhalte um.

**Nachtmodus**  
Im Nachmodus werden Karten mit weißer Schrift auf schwarzem Hintergrund angezeigt. Manche Kartenvorlagen
musst du vielleicht anpassen, damit sie in diesem Modus gut funktionieren. Siehe
[Nachtmodus-Design](templates/styling.md#night-mode) für weitere Informationen.

**Beim Hinzufügen aktuellen Stapel als Standard festlegen**  
Beeinflusst die Wechselwirkung zwischen Notiztypen und Stapeln. Das voreingestellte Verhalten
"Beim Hinzufügen aktuellen Stapel als Standard festlegen" bedeutet, dass Anki für jeden Stapel den
zuletzt genutzten Notiztyp speichert und ihn wieder auswählt, wenn du das nächste Mal den Stapel
auswählst. (Zusätzlich wird der aktuelle Stapel vorausgewählt, wenn du von irgendwo aus _Hinzufügen_
startest.)
Die andere Möglichkeit "Stapel abhängig vom Notiztyp zuweisen" speichert den zuletzt genutzten
Stapel für jeden Notiztyp (und der zuletzt genutzte Notiztyp wird vorausgewählt, wenn du _Hinzufügen_
startest). Das kann praktischer sein, wenn du für jeden Stapel immer einen einizigen Notiztyp verwendest.

**Standardmäßig eingestellter Suchtext**  
Erlaubt die Anpassung des anfänglichen Suchtextes in der Kartenverwaltung (`deck:current` lässt z.B.
den aktuellen Stapel anzeigen.)

**Schriftgröße der Benutzeroberfläche**  
Wenn dir die Elemente der Benutzeroberfläche zu klein sind, kannst du diese Einstellung erhöhen.

## Zeitplanung

**Zeit für nächste Wiederholung über Antworttaste anzeigen**  
Nützlich um zu wissen, wann Karten das nächste Mal wieder gezeigt werden

**Zähler für verbleibende Karten beim Lernen anzeigen**  
Deaktivieren, um den Kartenzähler am unteren Rand zu verstecken.

**Lernkarten mit größeren Lernstufen vor Wiederholungskarten zeigen**  
Nur mit aktiviertem V3-Zeitplaner sichtbar. Normalerweise werden Lernkarten mit einem Intervall
von mehr als einem Tag nach Wiederholungskarten gezeigt. Mit dieser Option werden sie stattdessen
vorher gezeigt.

**Veralteter Umgang mit Zeitzonen**  
Siehe
<https://faqs.ankiweb.net/timezone-handling-changes.html>.

**V3-Zeitplaner**  
Der V3-Zeitplaner ist hier dokumentiert:  
<https://faqs.ankiweb.net/the-2021-scheduler.html>

**Neue und Wiederholungskarten mischen**  
Nur mit V1- oder V2-Zeitplaner sichtbar. Diese Option bestimmt, wann neue Karten gezeigt werden:
Gemischt mit, vor oder nach Wiederholungskarten.

**Neuer Tag beginnt um**  
Legt fest, ab wann Anki die Karten des nächsten Tages zeigen soll. Die Standardeinstellung von 4 Uhr
stellt sicher, dass dir in einer Sitzung nicht die Karten von zwei Tagen angezeigt werden, wenn du
gegen Mittenacht lernst. Wenn du sehr spät schlafen gehst oder sehr früh aufstehst, solltest du
stattdessen eine Zeit einstellen, zu der du normalerweise schläfst.
Beachte, dass der Beginn des neuen Tages von deiner aktuellen Zeitzone abhängt. Beachte außerdem,
dass Karten, die eine Tagesgrenze überschreiten,
[zu Beginn des Tages, für den sie geplant wurden](./deck-options.md#day-boundaries),
angezeigt werden, genau wie Wiederholungskarten.

**Grenzwert für vorgezogenes Lernen**  
Bestimmt das Verhalten, wenn es im aktuellen Stapel nur noch Lernkarten zu lernen gibt.
Mit der Voreinstellung von 20 Minuten zeigt Anki Karten verfrüht, wenn ihr Restintervall weniger
als 20 Minuten beträgt und es sonst nichts zu tun gibt.
Wenn du 0 einstellst, wartet Anki immer das ganze Intervall ab und zeigt den Glückwunsch-Bildschirm,
bis die verbleibenden Karten bereit sind.

**Zeitbegrenzung für Sitzungen**  
_Timeboxing_ ist eine Konzentrationstechnik, bei der eine längere Aktivität (wie eine dreißigminütige
Lerneinheit) in kleinere Blöcke zerlegt wird. Wenn du eine Zeitbegrenzung von mehr als 0 Minuten
einstellst, zeigt Anki dir regelmäßig, wie viele Karten du in in der vorgegebenen Zeit geschafft hast.

## Netzwerk

Der Netzwerkreiter enthält Einstellungen für die Synchronisierung mit AnkiWeb.

- Wenn du angemeldet bist, wird eine Schaltfläche zum **Abmelden** angezeigt.
- Wenn die Option "Bei der nächsten Synchronisation Änderungen in eine Richtung erzwingen" aktiviert
  ist, wirst du bei der nächsten Synchronisierung gefragt, ob du hochladen oder herunterladen willst.
  Das ist nützlich, wenn du aus Versehen Änderungen vorgenommen hast und sie mit einer älteren Version
  auf AnkiWeb rückkgängig machen willst.
