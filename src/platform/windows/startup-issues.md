# Startprobleme

<!-- toc -->

## Windows-Updates

Wenn du Anki startest, erhältst du vielleicht eine solche Meldung:

- *Fehler beim Laden der Python-DLL.*
- *Das Programm kann nicht gestartet werden, weil api-ms-win-... nicht auf Ihrem
  Computer installiert ist.*
- *Skript runanki kann nicht ausgeführt werden.*
- *Skript pyi_rth_multiprocessing kann nicht ausgeführt werden.*
- *Skript pyi_rth_win32comgenpy kann nicht ausgeführt werden.*

Diese Fehlermeldungen erscheinen für gewöhnlich, weil deinem PC ein Windows-Update
oder eine Windows-Bibliothek fehlt.

Öffne bitte Windows Update und stell sicher, dass alle Updates installiert sind.
Falls welche installiert werden müssen, starte deinen PC bitte nach der Installation
neu.

## Windows 7/8

Auf Windows 7/8 musst du vielleicht manuell zusätzliche Updates installieren.
Versuche es bitte mit:

- <https://www.microsoft.com/en-us/download/details.aspx?id=48234>
- <https://aka.ms/vs/15/release/vc_redist.x64.exe>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4474419>
- <http://www.catalog.update.microsoft.com/Search.aspx?q=kb4490628>

## Videotreiber

Siehe bitte [Anzeigeprobleme](./display-issues.md).

## Mehrere Bildschirme

Wenn du die Meldung *"LoadLibrary ist mit Fehler 126 fehlgeschlagen"* bekommst,
könnte das daran liegen, dass das von Anki benutzte Toolkit Probleme mit
[mehreren Bildschirmen](https://forums.ankiweb.net/t/error-126-on-open-anki-desktop/13967)
hat.

## Antivirus- / Firewall-Software

Drittanbieter-Software auf deinem Rechner kann Anki am Starten hindern. Du kannst
versuchen, eine Ausnahme hinzuzufügen oder die Antivirus- / Firewall-Software
vorübergehend deaktivieren, um zu sehen, ob es hilft.

## Administratorrechte

Einige Nutzer haben berichtet, dass Anki erst gestartet hat, nachdem sie auf das
Anki-Symbol rechtsgeklickt und "Als Administrator ausführen" ausgewählt haben.
Anki speichert all seine Dateien in deinem Benutzerorder und sollte keine Administratorrechte
benötigen, aber es ist einen Versuch wert, wenn du die Alternativen ausgeschöpft hast.

## Mehrere Anki-Installationen nach Update

Wenn nach einem Update mehrere Anki-Installationen vorliegen (zum Beispiel in
`C:\Programme\Anki` and `C:\Programme (x86)\Anki`), könnten sie fehlerhaft
sein und Anki sich nicht ohne Fehlermeldung starten lassen.

Versuche, alle Kopien zu deinstallieren, zum Beispiel mit Windows' `Apps und Features`
oder, indem du `uninstall.exe` in jedem Anki-Ordner ausführst. Anschließend kannst
du Anki wieder installieren.

## Debuggen

Anki von der Konsole aus zu starten, kann weitere Erkenntnisse über einige Fehler
liefern. Nachdem du die neueste Anki-Version und alle Windows-Updates installiert
hast, kannst du Start>Ausführen>cmd.exe benutzen, anstatt Anki direkt zu starten.
Gib Folgendes in die geöffnete Konsole ein:

```bat
cd \program files\anki & anki-console
```

Vermutlich wird Anki genausowenig starten wie zuvor, aber es könnte Informationen
über die Fehlerursache liefern.

## Wenn alles andere versagt

Wenn du Anki immer noch nicht starten kannst, nachdem du alle obigen Vorschläge
ausprobiert hast, gibt es noch zwei verbleibende Optionen:

- Du kannst versuchen,
  [Anki von Python aus](https://faqs.ankiweb.net/running-from-python.html) zu starten.
- Du kannst eine ältere Anki-Version wie 2.1.35-alternate oder 2.1.15 ausprobieren,
  die mit einer anderen Version des Toolkits erstellt wurden.
