# Textgröße

Wenn du feststellst, dass der Text die falsche Größe hat, gibt es zwei Umgebungsvariablen,
die du ausprobieren kannst:

- `ANKI_NOHIGHDPI=1` deaktiviert teilweise Qt’s Unterstützung für hohe DPI.

- `ANKI_WEBSCALE=1` ändert die Skalierung von Ankis Web-Ansichten (wie die Stapelansicht,
  den Lernbildschirm etc.), wohingegen es Schnittstellen-Elemente wie die Menüleiste
  nicht verändert. Ersetze `1` mit der gewünschten Skalierung, wie `1.5` oder `0.75`.

In Windows kannst du diese Variablen zu einer Batch-Datei hinzufügen, um Anki leichter
starten zu können. Erstelle zum Beispiel eine Datei `startanki.bat` auf deinem
Desktop mit folgendem Inhalt:

```bat
set ANKI_WEBSCALE=0.75
start "Anki" "C:\Programme\Anki\anki"
```

Nach dem Speichern kannst du die Datei doppelklicken, um Anki mit dieser Einstellung
zu starten.
