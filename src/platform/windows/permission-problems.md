# Berechtigungsprobleme

Wenn du Fehlermeldungen wie "Zugriff verweigert" erhältst, sind einige Anki-Dateien
vielleicht schreibgeschützt, das heißt, Anki kann sie nicht verändern.

Um das Problem zu beheben, kannst du das Folgende tun:

- Gib `cmd.exe` in die Suchleiste des Startmenüs ein und drücke <kbd>Enter</kbd>.
- Gib `whoami` in das sich öffnende Fenster ein und drücke <kbd>Enter</kbd>,
  um deinen Benutzernamen anzuzeigen.
- Gib nun das Folgende ein, wobei du nach jeder Zeile <kbd>Enter</kbd> drückst und
  ____ (ohne das `:F` zu entfernen) mit deinem Benutzernamen ersetzt:
  ```bat
  cd %APPDATA%
  icacls Anki2 /grant ____:F /t
  ```

Dieser Befehl sollte die Zugriffsrechte in Ankis Dateiordner korrigieren und du
solltest nun in der Lage sein, das Programm zu starten.

## Antivirus / Firewall / Anti-Malware

Einige Nutzer haben Fehlermeldungen wie "Zugriff verweigert" oder "schreibgeschützt"
erhalten, die von Sicherheits-Software verursacht wurden. Möglicherweise musst du
eine Ausnahme für Anki hinzufügen oder die Software vorübergehend deaktivieren,
um sie als Verursacher ausschließen zu können.
Manche Nutzer haben berichtet, dass allein, die Software abzuschalten, nicht geholfen
hat und sie entweder eine Ausnahme für Anki hinzufügen oder die Software deinstallieren mussten.

## Berechtigungsprobleme finden und beseitigen

Wenn die Probleme weiterhin bestehen, nachdem du Antivirus- und ähnliche Programme
ausgeschlossen hast, die oben beschriebenen Schritte ausgeführt hast und nicht OneDrive
benutzt, führe bitte die folgenden Befehle in `cmd.exe` aus, indem du nach jeder Zeile
<kbd>Enter</kbd> drückst:
```bat
whoami
cd %APPDATA%
icacls Anki2 /t
```
Mache anschließend einen Screenshot von dem, was du siehst, oder kopiere es, und
schick es uns in einer Support-Anfrage.
