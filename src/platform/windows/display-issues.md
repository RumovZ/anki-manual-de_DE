# Anzeigeprobleme

Auf Windows gibt es drei Möglichkeiten, Inhalte auf dem Bildschirm anzuzeigen.
Der Standard ist *Software*, langsam aber am kompatibelsten. Es gibt zwei
Alternativen: *OpenGL* und *ANGLE*. Sie sind schneller, aber funktionieren vielleicht
nicht oder nicht richtig, was zu fehlenden Menüleisten, leeren Fenstern und so weiter
führen kann. Welche Option am besten funktioniert, hängt von deinem Computer ab.

Der Anzeigetreiber kann unter Werkzeuge>Einstellungen angepasst werden.
Anschließend solltest du Anki neu starten.

Wenn du nicht auf Ankis Einstellungen zugreifen kannst und Anki ein paar mal neu zu
starten nicht hilft, musst du den Grafiktreiber vielleicht manuell anpassen.
Dafür kannst cmd.exe starten und das Folgende eingeben:

```bat
echo auto > %APPDATA%\Anki2\gldriver
```

Die Voreinstellung ist `software`; die beiden anderen Treiber, die du ausprobieren kannst,
sind `angle` und `auto`.
