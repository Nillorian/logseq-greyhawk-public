# AGENTS - Regeln und Absichten fuer den Public Graph

## Intent
Dieser Graph ist fuer Spieler bestimmt. Ziel ist, veroeffentlichbare Informationen aus der Kampagne konsistent, sicher und nachvollziehbar bereitzustellen.

## Kontext
- Root: /home/nillorian/LogSeq/logseq-greyhawk-public
- Inhalte in pages/ sind oeffentlich.
- assets/ darf nur Material enthalten, das fuer Spieler freigegeben ist.
- Der private Kampagnen-Graph ist die Hauptquelle; dieser Graph ist ein kuratierter Auszug.

## Kernregeln
1. Keine DM-only Inhalte veroeffentlichen.
2. Keine geheimen Plotinfos, Loesungen oder versteckten Motivationen aufnehmen.
3. Keine internen UUIDs, privaten Backlinks oder Hinweise auf private Dateien teilen.
4. Nur freigegebene Bilder, Karten und Handouts unter assets/ referenzieren.
5. Bei Unsicherheit: nicht veroeffentlichen, sondern als draft markieren.

## Inhaltliche Leitplanken
1. Schreibe aus Spielerperspektive.
2. Trenne Fakt von Geruecht klar.
3. Nutze knappe, gut scannbare Abschnitte.
4. Halte Begriffe und Benennungen konsistent mit Templates.md.
5. Dokumentiere relevante Aenderungen in Sitzungs- oder Quest-Seiten.

## Seitenstatus
Nutze nach Moeglichkeit diese Properties:
- public:: true
- status:: draft | published
- spoiler:: none | low | medium
- type:: npc | location | faction | item | quest-hook | scene | session-note | statblock | dnd-pc

## Arbeitsablauf fuer Agenten
1. Quelle im privaten Graph identifizieren.
2. Nur sichere Inhalte in den Public Graph uebernehmen.
3. Seite mit passendem Template aus pages/Templates.md erstellen oder aktualisieren.
4. Quick-Check vor Abschluss:
   - Keine DM-only Abschnitte ausgefuellt
   - Keine privaten Verweise
   - Nur freigegebene Assets
5. Status auf published setzen, wenn alles geprueft ist.

## Erlaubte Eingriffe
- Strukturieren, kuerzen, sprachlich klarer machen
- Konsistente Properties und Tags setzen
- Oeffentliche Querverweise in pages/ pflegen

## Nicht erlaubte Eingriffe
- Inhalte aus privaten Notizen ungeprueft kopieren
- Spoiler in oeffentliche Kurzfassungen einbauen
- Verweise auf private Repositories oder lokale Dateipfade belassen

## Sicherheitscheckliste vor Commit
1. Suche nach Woertern wie "DM", "geheim", "intern", "Loesung", "Hinterhalt".
2. Pruefe neue Dateien auf unbeabsichtigte Metadaten.
3. Oeffne geaenderte Seiten aus Spielersicht und pruefe Verstaendlichkeit.

## Definition of Done
- Seite ist fuer Spieler verstaendlich.
- Keine sensiblen Informationen enthalten.
- Template-konform und sauber verlinkt.
- Status und Properties gesetzt.
