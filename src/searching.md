# Suchen

<!-- toc -->

Ankis Kartenverwaltung und die Auswahlstapelfunktion benutzen die gleiche
Methode, um nach bestimmten Karten oder Notizen zu suchen.

## Einfache Suchen

Wenn du Text in die Suchleiste eingibst, findet Anki passende Notizen und
zeigt ihre Karten. Anki sucht in allen Feldern der Notizen, aber nicht in ihren
Schlagwörtern (siehe dafür weiter unten). Ein paar Beispiele:

`hund`  
Sucht nach "Hund", findet auch Wörter wie "hundert" und "Wachhund".

`hund katze`  
Findet Notizen, die sowohl "Hund" als auch "Katze" beinhalten, z.B. "wie Hund und
Katze".

`hund or katze`  
Findet Notizen mit "Hund" _oder_ (Englisch "or") "Katze".

`hund (katze or maus)`  
Findet Notizen mit "Hund" und "Katze" oder mit "Hund" und "Maus".

`-katze`  
Findet Notizen _ohne_ das Wort "Katze".

`-katze -maus`  
Findet Notizen, die weder "Katze" noch "Maus" beinhalten.

`-(katze or maus)`  
Wie darüber.

`"ein hund"`  
Findet Notizen mit der exakten Buchstabenfolge "ein Hund" wie "mein Hund", aber
nicht "Hund ein" oder "einhundert".

`-"ein hund"`  
Findet Notizen ohne den exakten Ausdruck "ein Hund"

`h_nd`  
Findet Notizen mit "h", dann einem beliebigen Buchstaben und dann "nd", z.B.
"Hund" und "Hand".

`h*nd`  
Findet Notizen mit "h", dann beliebigen Buchstaben und dann "nd" wie "hnd",
"Hund", "hängend" usw.

`w:hund`  
Sucht nach "Hund" umgeben von Wortgrenzen, z.B. "Hund, der", aber nicht "hundert" oder
"Wachhund". Benötigt Anki 2.1.24+ oder AnkiMobile 2.1.61+. Beachte, dass Formatierungsänderungen
als Wortgrenzen interpretiert werden. Z.B. findet `w:Bei` den Text Bei**spiel**. 

`w:hund*`  
Findet "Hund" und "hundert", aber nicht "Wachhund".

`w:*hund`  
Findet "Hund" und "Wachhund", aber nicht "hundert".

An diesen Beispielen lässt sich Folgendes beobachten:

- Suchbegriffe werden durch Leerzeichen getrennt.

- Wenn mehrere Suchebegriffe angegeben werden, sucht Anki nach Notizen mit ihnen allen -
  ein implizites `and` ("und") wird zwischen je zwei Begriffen eingefügt. In Anki 2.1.24+
  und AnkiMobile 2.0.60+ kannst du das explizit angeben, wenn du möchtest (`hund and katze` ist
  das gleiche wie `hund katze`), aber ältere Anki-Versionen werden `and` einfach wie einen
  weiteren Suchbegriff behandeln.

- Du kannst `or` benutzen, wenn nur einer von zwei Suchbegriffen passen muss.

- Du kannst `-`, ein Minus, voranstellen, um Notizen zu finden, die nicht passen.

- Du kannst Suchbegriffe gruppieren, indem du sie einklammerst, wie im Beispiel `hund (katze or maus)`.
  Das ist wichtig, wenn du `or` und `and` kombinierst. Das Beispiel findet Notizen mit "Hund Katze"
  oder "Hund Maus", aber ohne die Klammern würde es Notizen mit "Hund Katze" oder "Maus" finden.

- Anki kann innerhalb Formatierung nur im eingestellten [Sortierfeld](editing.md#customizing-fields)
  suchen. Wenn du in einem Feld z.B. "**Bei**spiel" schreibst, wird Anki diese Notiz bei einer Suche
  nach `beispiel` nicht finden, es sei denn, es handelt sich um das Sortierfeld.
  Ändert sich die Formatierung eines Wortes nicht zwischendrin, kann Anki dieses Wort in jedem beliebigen
  Feld finden.

- Einfache Suchen ignorieren Groß-/Kleinschreibung von lateinischen Buchstaben: a-z impliziert A-Z
  und umgekehrt. Für andere Buchstaben wie Umlaute gilt das nicht: `Öl` findet keine Notizen mit "ölig".
  Um auch hier Groß-/Kleinschreibung zu ignorieren, können die Suchen nach Wortgrenzen oder regulären
  Ausdrücken genutzt werden (`w:`, `re:`).

## Eingrenzung auf Felder

Du kannst Anki auch nur in einem bestimmten Feld suchen lassen. Anders als die Suchen oben erfordert
diese Variante eine exakte Übereinstimmung.

`vorderseite:hund`  
Findet Notizen mit einem Feld _Vorderseite_, das genau "Hund" enthält. Ein Feld mit Inhalt "ein Hund"
würde nicht gefunden werden.

`"Mein Tier:ein Hund"`  
Findet Notizen, wo das Feld "Mein Tier" genau "ein Hund" enthält. Die Anführungszeichen sind
erforderlich, siehe [unten](#matching-special-characters).

`vorderseite:*hund*`  
Findet Notizen mit einem Feld _Vorderseite_, in dem irgendwo "Hund" vorkommt.

`vorderseite:`  
Findet Notizen mit einem leeren Feld _Vorderseite_.

`vorderseite:_*`  
Findet Notizen mit einem nicht leeren Feld _Vorderseite_.

`vorderseite:*`  
Findet Notizen mit einem Feld _Vorderseite_, egal ob leer oder nicht.

`vor*:text`  
Findet Notizen mit einem Feld, das mit mit "Vor" beginnt. Benötigt Anki 2.1.24+ oder AnkiMobile 2.1.60+.

## Schlagwörter, Stapel, Karten- und Notiztypen

`tag:tier`  
Findet Notizen mit dem Schlagwort "Tier" oder einem Unterschlagwort wie "Tier::Säugetier".

`tag:none`  
Findet Notizen ohne Schlagwörter.

`tag:ti*`  
Findet Notizen mit Schlagwörtern, die mit "Ti" beginnen.

`deck:französisch`  
Findet Karten in dem Stapel _Französisch_ oder in einem Unterstapel wie _Französisch::Vokabeln_.

`deck:französisch -deck:französisch::*`  
Findet Karten in dem Stapel _Französisch_, aber nicht in seinen Unterstapel.

`deck:"vokabeln französisch"`  
Für Stapelnamen mit Leerzeichen.

`"deck:vokabeln französisch"`  
Alternative zu oben.

`deck:filtered`  
Nur Auswahlstapel.

`-deck:filtered`  
Nur reguläre Stapel.

`card:vorwärts`  
Findet Karten mit dem Kartentyp _Vorwärts_.

`card:1`  
Findet Karten mit Kartentyp Nummer 1. Um z.B. die Karte mit dem zweiten Lückentext einer Notiz zu
finden, könntest du `card:2` benutzen.

`note:einfach`  
Findet Notizen mit dem Notiztyp _Einfach_.

## Akzente / kombinierende Zeichen ignorieren

Benötigt Anki 2.1.24+ oder AnkiMobile 2.0.60+.

Du kannst `nc:` benutzen, um kombinierende Zeichen zu ignorieren (für Englisch "*n*o *c*ombining").
Beispiel:

`nc:uber`  
Findet Notizen mit "uber", "über", "Über" usw.

`nc:は`  
Findet "は", "ば" und "ぱ".

Diese Suchen sind langsamer als reguläre Suchen.

## Reguläre Ausdrücke

Anki 2.1.24+ und AnkiMobile 2.0.60+ unterstützen die Suche mit _regulären Ausdrücken_, einem
standardisierten und mächtigen Verfahren, um Text zu durchsuchen.

Beginne eine Suche dafür mit `re:`. Zur Erleichterung wird Anki das Folgende als [Roheingaben](#raw-input)
betrachten, also beachte die dort aufgelisteten Regeln.

Beispiele:

`"re:(k|irgend).*ein"`  
Findet Notizen, die "k" oder "irgend" beinhalten, dann 0 oder mehr beliebige Zeichen und schließlich "ein".

`re:\d{3}`  
Findet Notizen mit drei Zahlen hintereinander.

Reguläre Ausdrücke können ebenfalls auf ein Feld eingegrenzt werden. Bitte beachte, dass das anders
als normale Suchen keine exakte Übereinstimmung erfordert. Beispiel:

`vorderseite:re:[a-c]1`  
Findet "a1", "b1" und "c1", auch groß geschrieben, irgendwo in einem Feld _Vorderseite_.

`front:re:^[a-c]1$`  
Wie oben, erfordert aber, dass vor und nach "a1", "b1" bzw. "c1" kein weiterer Text steht.

Seit Anki 2.1.50 können reguläre Ausdrücke auch für Schlagwörter benutzt werden:

`tag:re:^vorfahr$`  
Findet Notizen mit dem exakten Schlagwort "Vorfahr", ohne Unterschlagwörter wie "Vorfahr::Nachfahre"
zu berücksichtigen.

`"tag:re:lektion-(1[7-9]|2[0-5])"`  
Findet Notizen mit den Schlagwörtern "Lektion-17" bis "Lektion-25".

Mehr über reguläre Ausdrücke findest du z.B. hier:
<https://www.ionos.de/digitalguide/websites/webseiten-erstellen/regulaere-ausdruecke/>

Ein paar Anmerkungen:

- Standardmäßig ignoriert die Suche Groß-/Kleinschreibung. Durch das Voranstellen von `(?-i)` kann
  das geändert werden.
- Manche Zeichen wie Zeilenumbrüche oder Leerzeichen werden in HTML anders dargestellt. Du kannst
  den HTML-Editor des Editor-Fensters benutzen, um das zugrundeliegende HTML zu sehen.
- Für Details zu den von Anki unterstützten regulären Ausdrücken, siehe die Dokumentation des Crates _regex_:
  <https://docs.rs/regex/1.3.9/regex/#syntax> (Englisch)

## Kartenstatus

`is:due`  
Fällige Wiederholungs- und Lernkarten.

`is:new`  
Neue Karten.

`is:learn`  
Lernkarten.

`is:review`  
Wiederholungskarten (fällig oder nicht), auch gescheiterte.

`is:suspended`  
Karten, die manuell ausgesetzt wurden.

`is:buried`  
Karten, die entweder [automatisch](studying.md#siblings-and-burying) oder manuell zurückgestellt wurden.

Beachte, dass der neue [Zeitplaner](https://faqs.ankiweb.net/the-anki-2.1-scheduler.html) zwischen
manuell und automatisch zurückgestellten Karten unterscheidet, sodass du die einen ohne die anderen
wiedereinstellen kannst.

Karten, deren Wiederholung gescheitert ist, fallen in mehrere dieser Kategorien, weshalb es nützlich
sein kann, Kombinationen von ihnen zu verwenden, um genauere Ergebnisse zu erzielen:

`is:learn is:review`  
Gescheiterte Karten, die in der Wiedererlernphase sind.

`-is:learn is:review`  
Wiederholungskarten, aber keine gescheiterten.

`is:learn -is:review`  
Karten, die erstmalig gelernt werden.

`flag:1`  
Karten mit der roten Markierung.

`flag:2`  
Karten mit der orangen Markierung.

`flag:3`  
Karten mit der grünen Markierung.

`flag:4`  
Karten mit der blauen Markierung.

`flag:5`  
Karten mit der rosa Markierung.

`flag:6`  
Karten mit der türkisen Markierung.

`flag:7`  
Karten mit der lilanen Markierung.

## Karteneigenschaften

`prop:ivl>=10`  
Karten mit einem Intervall von 10 Tagen oder mehr.

`prop:due=1`  
Karten, die morgen fällig sind.

`prop:due=-1`  
Gestern fällige Karten, die noch nicht beantwortet wurden.

`prop:due>-1 prop:due<1`  
Karten, die zwischen gestern und morgen fällig sind.

`prop:reps<10`  
Karten, die seltener als zehn mal beantwortet wurden.

`prop:lapses>3`  
Karten, die öfter als drei mal gescheitert sind.

`prop:ease!=2.5`  
Karten, die schwieriger oder leichter sind als der Standardwert.

## Jüngste Ereignisse

### Hinzugefügt

`added:1`  
Heute hinzugefügte Karten.

`added:7`  
In der letzten Woche hinzugefügte Karten.

Dieses Kriterium prüft das Datum der Karten-, nicht der Notizerstellung. Daher werden kürzlich erstellte
Karten eingeschlossen, auch wenn ihre Notizen schon vor langer Zeit hinzugefügt wurden.

### Bearbeitet

`edited:3`  
Karten, deren Notiztext in den letzten drei Tagen hinzugefügt oder bearbeitet wurde.

Anki 2.1.28+ / AnkiMobile 2.0.64+ wird benötigt.

### Beantwortet

`rated:1`  
Heute beantwortete Karten.

`rated:1:2`  
Heute mit _Schwer_ (2) beantwortete Karten.

`rated:7:1`  
In der letzten Woche mit _Nochmal_ (1) beantwortete Karten.

`rated:31:4`  
Im letzten Monat mit _Einfach_ (4) beantwortete Karten.

Vor Version 2.1.39 war diese Suche auf 31 Tage begrenzt.

### Erstmalig beantwortet

Mit Version 2.1.45+ lässt sich auch gezielt nach der allerersten Beantwortung suchen:

`introduced:1`  
Karten, die heute das erste Mal beantwortet wurden.

`introduced:365`  
Karten, die das erste Mal in den letzten 365 Tagen beantwortet wurden.

## Nach Sonderzeichen suchen

Dieser Abschnitt wurde für Anki 2.1.36+ geschrieben - in früheren Versionen war das Maskieren von
Sonderzeichen in bestimmten Fällen nicht möglich.

Wie bereits gesehen haben manche Zeichen wie `*`, `_` oder `"` eine besondere Bedeutung in Anki.
Wenn du diese Zeichen mit einer Suche ausfindig machen willst, musst du Anki anweisen, sie nicht
besonders zu behandeln.

- _Leerzeichen_  
  Um etwas mit Leerzeichen zu finden, muss der `"gesamte Ausdruck"` in Anführungszeichen gesetzt werden.
  Bei einer Doppelpunktsuche kann auch nur der `Teil:"nach dem Doppelpunkt"` umfasst werden,
  solange der Teil vor dem Doppelpunkt keine Leerzeichen enthält.

- `"`, `*` und `_`  
  Stell diesen Zeichen einen umgekehrten Schrägstrich voran, um nach ihnen zu suchen. Z.B. findet
  `_` ein einzelnes beliebiges Zeichen, aber `\_` nur den Unterstrich.

- `\`  
  Da der umgekehrte Schrägstrich benutzt wird, um Zeichen ihre besondere Bedeutung zu nehmen, wird
  auch er gesondert behandelt. Um nach dem Zeichen an sich zu suchen, kannst du `\\` statt `\` benutzen.

- `(` und `)`  
  Um nach Klammern zu suchen, kann entweder der gesamte Ausdruck in Anführungszeichen gesetzt und/oder
  ein umgekehrter Schrägstrich verwendet werden. D.h. `"ein(Wort)"`, `ein\(Wort\)` und
  `"ein\(Wort\)"` bedeuten alle das Gleiche, aber `ein(Wort)` nicht.

- `-`  
  Einen Ausdruck mit `-` zu beginnen, kehrt ihn normalerweise um: `-hund` findet alles außer "Hund".
  Wenn du einen Bindestrich selbst finden willst, kannst du entweder einen umgekehrten Schrägstrich
  verwenden oder den gesamten Ausdruck in Anführungszeichen setzen: `\-.-` oder `"-.-"`.

- `:`  
  Doppelpunkte müssen maskiert werden, außer es steht bereits davor ein unmaskierter Doppelpunkt.
  `w:e:g` ist also eine Wortgrenzensuche nach `e:g`, `w\:e\:g` findet buchstäblich `w:e:g` und `w\:e:g`
  sucht in einem Feld `w:e` nach `g` (siehe [Eingrenzung auf Felder](#limiting-to-a-field)).

- `&`, `<` und `>`  
  `&`, `<` und `>` werden beim Suchen als HTML behandelt, weshalb Suchen mit ihnen nicht wie erwartet
  funktionieren. Du kannst nach ihnen aber mithilfe ihrer HTML-Entität-Namen suchen (`&amp;` für `&`,
  `&lt;` für `<` und `&gt;` für `>`). Z.B. findet `&lt;&amp;text&gt;` Notizen mit `<&text>` in einem
  Feld.

### Roheingaben

Nach bestimmten Schlüsselwörtern (wie `re:`) wird folgender Text als Roheingabe behandelt.
Das bedeutet, die oben aufgelisteten Sonderzeichen verlieren zum Großteil ihre besondere Bedeutung.
Nur ein Minimum an Maskierung ist notwendig, um Mehrdeutigkeit zu vermeiden:

- `"` muss maskiert werden.

- Leerzeichen und unmaskierte Klammern erfordern, dass der Ausdruck in Anführungszeichen gesetzt wird.

- Ein Ausdruck darf nicht in einer ungeraden Anzahl von umgekehrten Schrägstrichen enden.

## Kennnummern

`nid:123`  
Die Notiz mit Kennnummer 123.

`cid:123,456,789`  
Die Karten mit Kennnummern 123, 456 oder 789.

Notiz- und Kartenkennnummern werden in der [Kartenstatistik](stats.md) angezeigt.
Diese Suchen können bei der Add-on-Entwicklung oder anderen datenbanknahen Arbeiten nützlich sein.
