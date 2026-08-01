# AGENTS - Regeln und Absichten für das Public Repository

## Intent
Dieses Repository ist für Spieler bestimmt. Ziel ist, veröffentlichbare Informationen aus der Kampagne konsistent, sicher und nachvollziehbar bereitzustellen.

## Kontext
- Root: /home/nillorian/LogSeq/logseq-greyhawk-public
- Inhalte in pages/ sind öffentlich.
- assets/ darf nur Material enthalten, das für Spieler freigegeben ist.
- Der private Kampagnen-Quellbereich ist die Hauptquelle; dieses Repository ist ein kuratierter Auszug.

## Kernregeln
1. Keine DM-only Inhalte veröffentlichen.
2. Keine geheimen Plotinfos, Lösungen oder versteckten Motivationen aufnehmen.
3. Keine internen UUIDs, privaten Backlinks oder Hinweise auf private Dateien teilen.
4. Nur freigegebene Bilder, Karten und Handouts unter assets/ referenzieren.
5. Bei Unsicherheit: nicht veröffentlichen, sondern als draft markieren.

## Inhaltliche Leitplanken
1. Schreibe aus Spielerperspektive.
2. Trenne Fakt von Gerücht klar.
3. Nutze knappe, gut scannbare Abschnitte.
4. Halte Begriffe und Benennungen konsistent mit Templates.md.
5. Dokumentiere relevante Änderungen in Sitzungs- oder Quest-Seiten.
6. Verwende korrektes Deutsch mit Umlauten und ß auf öffentlichen Seiten.

## Seitenstatus und Metadatenformat
Verwende in öffentlichen Seiten einen sichtbaren Metadaten-Abschnitt statt Logseq-Properties.

Empfohlenes Format direkt unter der H1-Überschrift:
- **Typ**: npc | location | faction | item | quest-hook | scene | session-note | statblock | dnd-pc
- **Sichtbarkeit**: public
- **Status**: draft | published
- **Spoiler-Level**: none | low | medium
- **Tags**: kommagetrennte Schlagworte

Beispiel:
- **Typ**: npc
- **Sichtbarkeit**: public
- **Status**: published
- **Spoiler-Level**: none
- **Tags**: greyhawk-campaign, npc

## Arbeitsablauf für Agenten
1. Quelle im privaten Kampagnenbereich identifizieren.
2. Nur sichere Inhalte in das Public Repository übernehmen.
3. Seite mit passendem Template aus pages/Templates.md erstellen oder aktualisieren.
4. Quick-Check vor Abschluss:
   - Keine DM-only Abschnitte ausgefüllt
   - Keine privaten Verweise
   - Nur freigegebene Assets
5. Status auf published setzen, wenn alles geprüft ist.

## Erlaubte Eingriffe
- Strukturieren, kürzen, sprachlich klarer machen
- Konsistente Properties und Tags setzen
- Öffentliche Querverweise in pages/ pflegen

## Nicht erlaubte Eingriffe
- Inhalte aus privaten Notizen ungeprüft kopieren
- Spoiler in öffentliche Kurzfassungen einbauen
- Verweise auf private Repositories oder lokale Dateipfade belassen

## Sicherheitscheckliste vor Commit
1. Suche nach Wörtern wie "DM", "geheim", "intern", "Lösung", "Hinterhalt".
2. Prüfe neue Dateien auf unbeabsichtigte Metadaten.
3. Öffne geänderte Seiten aus Spielersicht und prüfe Verständlichkeit.

## Pre-Push Pflichtcheck
Vor jedem Push auf `main` zusätzlich die Freigabe- und Copyright-Regeln prüfen:

- `docs/PUBLIC-CONTENT-RULES.md`

## Definition of Done
- Seite ist für Spieler verständlich.
- Keine sensiblen Informationen enthalten.
- Template-konform und sauber verlinkt.
- Status und Properties gesetzt.
