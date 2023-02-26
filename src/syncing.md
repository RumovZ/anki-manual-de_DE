# Synchronisation mit AnkiWeb

<!-- toc -->

AnkiWeb ist ein Dienst, um deine Sammlung über verschiedene Geräte hinweg synchron
zu halten und online zu lernen. Bitte leg einen [kostenlosen Account](https://ankiweb.net/)
an, bevor du die folgenden Schritten durchführst.

## Einführungsvideos

Für eine schnelle Einführung in die Synchronisation sieh dir bitte die
[Einführungsvideos zur Synchronisation](https://www.youtube.com/watch?v=YkiM4DPzSVc&list=PLGgmaKOIHykFoomqkBJAyGiDQ2kyiuTao&yt:cc=on)
(englisch) an.

## Einrichtung

Um mit der geräteübergreifenden Synchronisation zu beginnen, klick auf die
Synchronisieren-Schaltfläche (oben rechts im Hauptbildschirm) oder drück <kbd>Y</kbd>
auf deiner Tastatur.
Du wirst nach deiner AnkiWeb-ID und deinem Passwort gefragt, die du bei der
Account-Erstellung angelegt hast.

Wenn du deine Sammlung das erste Mal synchronisierst, fragt dich Anki, ob du hoch-
oder herunterladen möchtest. Wenn du Karten auf deinem Computer hast und dein
AnkiWeb-Account leer ist, wähle _Hochladen_, um deine Kartendaten nach AnkiWeb
zu senden. Wenn du auf AnkiWeb Karten von einem anderen Gerät und keine auf deinem
Computer hast, wähle _Herunterladen_, um deine lokale leere Sammlung mit den Karten
von AnkiWeb zu ersetzen. Wenn du verschiedene Karten auf beiden Geräten hast, ist
[mehr Arbeit](#merging-conflicts) erforderlich, um den Verlust von Daten zu vermeiden.

Nachdem die erstmalige Einweg-Synchronisation abgeschlossen ist, kann Anki Änderungen
von mehreren Quellen mit ein paar Ausnahmen selbst zusammenführen.

Wenn mehrere Leute Anki auf demselben Gerät mit jeweils eigenem Profil nutzen,
muss jeder Benutzer seinen eigenen Account für die Synchronisation anlegen.
Wenn du versuchst, mehrere Profile mit demselben Account zu synchronisieren, wirst
du Daten verlieren.

## Automatische Synchronisation

Nachdem die Synchronisation einmal aktiviert ist, wird Anki deine Sammlung bei jedem
Öffnen und Schließen automatisch synchronisieren. Wenn du lieber manuell synchronisieren
möchtest, kannst du die automatische Synchronisation in den Einstellungen deaktivieren.

## Schaltflächenfarbe

Die Synchronisieren-Schaltfläche wird blau, wenn eine normale, und rot, wenn eine
volle Synchronisation erforderlich ist.

## Medien

Zugehöriges Video (englisch): <https://www.youtube.com/watch?v=phP9GGG-PxY>

Anki synchronisiert alle von deinen Notizen genutzten Audio- und Bilddateien.
Es registriert, wenn Dateien zu deinem Medienordner hinzugefügt oder daraus
entfernt worden sind, aber nicht, wenn du existierende Dateien verändert hast.
Dafür musst du erst auch eine Datei hinzugefügen oder entfernen.

Wenn du Anki von einem USB-Speicher aus startest, solltest du ein NTFS-Dateisystem
benutzen, da Anki Änderungen auf einem FAT32-System möglicherweise nicht registriert.

## Konflikte

Zugehöriges Video (englisch): <https://www.youtube.com/watch?v=UEAcpfMQnjo>

Unter normalen Umständen können Wiederholungen und Bearbeitungen zusammengeführt
werden. Wenn du Karten also auf zwei verschiedenen Geräten lernst und bearbeitest,
bevor du synchronisierst, übernimmt Anki die Änderungen von beiden Quellen.
Wenn dieselbe Karte an zwei verschiedenen Orten wiederholt wurde, werden beide
Wiederholungen in der Wiederholungshistorie vermerkt und die Karte verbleibt im
Zustand nach der aktuellsten Wiederholung.

Bestimmte Änderungen kann Anki nicht zusammenführen, hauptsächlich wenn sie das
Notizformat betreffen, z.B. das Hinzufügen eines Felds oder das Entfernen einer Vorlage.
Wenn du eine Aktion ausführst, die nicht zusammengeführt werden kann, warnt Anki
dich und gibt dir die Möglichkeit, sie abzubrechen. Wenn du trotzdem fortfährst,
wirst du bei der nächsten Synchronisation gefragt, ob du die lokale oder die Sammlung
auf AnkiWeb behalten möchtest.

Auch bestimmte Probleme beim Synchronisieren erzwingen eine Einweg-Synchronisation.
Wenn das häufiger geschieht, melde es bitte in unserem Forum.

Bei einer Einweg-Synchronisation musst du wählen, ob du deine lokale Sammlung
oder die auf AnkiWeb behalten möchtest. Wenn in beiden Änderungen vorgenommen
wurden, können nur die aus einer Quelle erhalten werden.

Wenn du _Hochladen_ wählst, wird der Inhalt deines lokalen Geräts nach AnkiWeb
geschickt. Danach musst du deine anderen Geräte synchronisieren und _Herunterladen_
wählen, damit sie diesen Inhalt kopieren.

Wenn du _Herunterladen_ wählst, werden alle lokalen Änderungen, die du vorgenommen
hast, durch die Daten von AnkiWeb ersetzt.

Nachdem alle Geräte synchronisiert sind, werden bei folgenden Synchronisationen
wieder Änderungen von beiden Seiten zusammengeführt.

Wenn du ein vollständiges Hoch- oder Herunterladen erzwingen möchtest (z.B. weil
du aus Versehen einen Stapel auf einer Seite gelöscht hast und ihn wiederherstellen
möchtest, anstatt seine Löschung zu synchronisieren), kannst du unter
_Werkzeuge > Einstellungen > Netzwerk_ den Haken bei "Bei der nächsten Synchronisation
Änderungen in eine Richtung erzwingen" setzen und dann wie gewohnt synchronisieren.
(Du hast dann die Wahl, welche Seite du benutzen willst.)

Änderungen in eine Richtung zu erzwingen, beeinflusst nur die Kartensynchronisation
– Medien werden wie immer synchronisiert. Wenn du Dateien von AnkiWeb entfernen
möchtest, stell bitte zuerst sicher, dass dein Gerät vollständig synchronisiert ist.
Anschließend werden alle Dateien, die du entfernst (z.B. durch die Funktion
_Medien überprüfen_), bei der nächsten Synchronisation von AnkiWeb entfernt.

## Zusammenführungskonflikte

Da die [erste Synchronisierung](#einrichtung) Änderungen nur in eine Richtung synchronisieren kann,
geht Inhalt, den du auf anderen Geräten oder Profilen hinzugefügt hast, verloren, wenn
du ihn mit dem Inhalt des anderen Geräts überschreibst. Mit etwas Arbeit ist es jedoch möglich,
Daten manuell zu einer einzigen Sammlung zusammenzuführen.

Beginne damit, auf jedem Gerät/Profil ein Backup zu erstellen, für den Fall, dass etwas schief geht. In der
Computer-Version kannst du unter Datei&gt;Export "Alle Stapel" mit Zeitplaninformationen und
Mediendateien exportieren und die Datei an einem sicheren Ort speichern. In AnkiMobile kannst du
über die Schaltfläche "Hinzufügen/Exportieren" in der Stapelübersicht Stapel mit
Medien exportieren.

Falles eines ein mobiles Gerät ist, synchronisiere es nun zuerst. Wenn es Konflikte gibt, wähle "Hochladen",
um vorhandene Daten auf AnkiWeb mit den Daten deines Mobilgeräts zu überschreiben. Wenn sich
beide Geräte/Profile auf deinem Computer befinden, synchronisiere zuerst das Gerät/Profil mit der
höchsten Anzahl an Stapeln.

Kehre nun zum anderen Gerät/Profil zurück. Wenn die automatische Synchronisierung aktiviert ist,
kann eine Meldung erscheinen, die fragt, ob du hoch- oder herunterladen möchtest. Klicke auf
die Abbrechen-Schaltfläche - noch möchten wir nicht synchronisieren.

Sobald du die Stapelübersicht siehst, klicke auf das Zahnradsymbol neben dem ersten Stapel und wähle
"Exportieren". Exportiere mit Zeitplaninformationen und Medien und speichere die
.apkg-Datei. Wiederhole diesen Schritt für jeden Oberstapel.

Sobald alle Oberstapel exportiert wurden, klick auf die Synchronisierungsschaltfläche oben rechts und
wähle "Herunterladen", um den lokalen Inhalt mit dem Inhalt zu überschreiben, den du von deinem
anderen Gerät synchronisiert hast.

Du kannst nun über Datei&gt;Importieren die .apkg-Dateien importieren, die du zuvor exportiert hast.
Dadurch wird der exportierte Inhalt mit dem vorhandenen Inhalt zusammengeführt, sodass alles an
einem Ort ist.

## Firewalls

Zur Synchronisation muss Anki in der Lage sein, ausgehende HTTPS-Verbindungen
nach ankiweb.net, sync.ankiweb.net, sync2.ankiweb.net und so weiter aufzubauen.
Diese Domains ändern und auch die IP-Adressen, auf die sie verweisen, können sich im
Laufe der Zeit ändern. Daher empfehlen wir, Wildcard-Zugriff auf \*.ankiweb.net zu erlauben,
um die Chance zu verringern, dass die Firewall-Regeln in Zukunft aktualisiert werden müssen.

Wenn du eine Firewall auf deinem Rechner hast, solltest du eine Ausnahme für
Anki hinzufügen. Wenn du dich in einem Arbeits- oder Schulnetzwerk befindest,
bitte deinen Netzwerkadministrator um Unterstützung - damit können wir nicht helfen.

## Proxies

Wenn du einen Proxy benötigst, um auf das Internet zuzugreifen, sollte Anki
automatisch deine System-Proxy-Einstellungen übernehmen, wenn du Windows oder
macOS verwendest. Wenn du auf einer anderen Plattform bist, wird die
HTTP_PROXY-Umgebungsvariable berücksichtigt.

Anki kann deine Systemeinstellungen nur dann übernehmen, wenn ein Proxy manuell
konfiguriert ist und kein Passwort erfordert. Wenn dein System eine automatische
Proxy-Konfiguration verwendet oder ein Proxy, der einen Benutzernamen und ein
Passwort erfordert, musst du Anki die Proxy-Konfiguration manuell mitteilen.

Um Anki deine Proxy-Einstellungen mitzuteilen, musst du die Umgebungsvariable HTTPS_PROXY
definieren, sodass sie auf den Proxy-Server zeigt. Das sieht etwa so aus:

    http://user:pass@proxy.company.com:8080

Wenn dein Benutzername oder Passwort ein @ enthält (z.B. `user@workdomain.com`),
musst du es durch %40 ersetzen, also:

    http://user%40workdomain.com:pass@proxy.company.com:8080

Anki 2.0 erwartet HTTP_PROXY anstelle von HTTPS_PROXY.

Um Umgebungsvariablen unter Windows zu setzen, siehe
<https://www.google.com/search?q=windows+set+environmental+variable>

Wenn du auf einem Mac bist, siehe
<http://stackoverflow.com/questions/135688/setting-environment-variables-in-os-x>

Stark eingeschränkte Netzwerke, die sichere Verbindungen abfangen und anstelle
eines Zertifikats ihr eigenes Zertifikat präsentieren, können dazu führen, dass
Anki SSL-Fehler ausgibt. In solchen Umgebungen kannst du die Fehler möglicherweise
mit <https://ankiweb.net/shared/info/878367706> umgehen.

Eine alternative Lösung besteht darin, einen lokalen Proxy-Server zu installieren
und diesen auf deinen normalen Proxy-Server zu verweisen. Du kannst Anki dann sagen,
dass es den lokalen Proxy verwenden soll, der Anfragen an den von dir normalerweise
verwendeten Proxy umleitet.
