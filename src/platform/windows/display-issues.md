# Anzeigeprobleme

<!-- toc -->

Auf Windows gibt es drei Möglichkeiten, Inhalte auf dem Bildschirm anzuzeigen.
Der Standard ist _Software_, langsam aber am kompatibelsten. Es gibt zwei
Alternativen: _OpenGL_ und _ANGLE_. Sie sind schneller, aber funktionieren vielleicht
nicht oder nicht richtig, was zu fehlenden Menüleisten, leeren Fenstern und so weiter
führen kann. Welche Option am besten funktioniert, hängt von deinem Computer ab.

Ob und wie du diese Anzeigeweise ändern kannst, hängt von der Anki-Version ab, die du benutzt,
genauer gesagt von der Version des benutzten Qt-Toolkits.

## Qt5

Dieses Toolkit wird von allen Anki-Versionen vor 2.1.50 benutzt. Hier kann der
Anzeigetreiber unter Werkzeuge>Einstellungen angepasst werden.
Anschließend solltest du Anki neu starten.

Wenn du nicht auf Ankis Einstellungen zugreifen kannst und, Anki ein paar mal neu zu
starten, nicht hilft, musst du den Grafiktreiber vielleicht manuell anpassen.
Dafür kannst du cmd.exe starten und das Folgende eingeben:

```bat
echo auto > %APPDATA%\Anki2\gldriver
```

Es wird kein Text ausgegeben. Nun kannst du Anki neu starten.

Die Voreinstellung ist `software`; die beiden anderen Treiber, die du ausprobieren kannst,
sind `angle` und `auto`.

## Qt6

Anki 2.1.50+ kann mit dem neueren Qt6-Toolkit benutzt werden. Grafikbeschleunigung ist hier
standardmäßig aktiviert. Bei Anzeigeproblemen kannst du den Modus `software` ausprobieren:

```bat
echo software > %APPDATA%\Anki2\gldriver6
```

Es wird kein Text ausgegeben. Nun kannst du Anki neu starten.

Um zur Standardeinstellung zurückzukehren, ersetze `software` durch `auto` oder lösch die Datei.

## Vollbild

Anki 2.1.50+ hat einen Vollbildmodus, der aber aufgrund verschiedener Probleme deaktiviert werden
musste, während `OpenGL` benutzt wird. Wird wie oben beschrieben zur `software`-Anzeige gewechselt,
kann der Vollbildmodus benutzt werden, aber bitte beachte, dass die Anzeigeleistung darunter leiden kann.
