# Greyhawk Public Spielerbereich

Website (Spieleransicht):
https://nillorian.github.io/logseq-greyhawk-public/

## Zweck
Dieses Repository enthaelt oeffentliche, spoilerarme Kampagneninhalte fuer Spieler.

## Eigenen Content hochladen (kurz)

### 1) Seite anlegen oder bearbeiten
- Neue Spielerseite unter pages/players/Name.md anlegen.
- Uebersichtsseiten liegen z. B. unter pages/players.md oder pages/contents.md.
- Bilder/Dateien fuer Spieler unter pages/assets/ ablegen und in der Seite verlinken.

### 2) Format beachten
- Vorlage und Feldnamen: pages/Templates.md
- Keine Logseq-Properties wie type::, tags::, status:: in oeffentlichen Seiten nutzen.
- Stattdessen sichtbare Metadaten direkt unter der H1 verwenden.

### 3) Sicherheits- und Copyright-Check
- Vor dem Push immer pruefen: docs/PUBLIC-CONTENT-RULES.md
- Keine DM-only Infos, keine geheimen Loesungen, keine unklar lizenzierten Assets.

### 4) Aenderungen hochladen (lokal per Git)
- git add .
- git commit -m "Add or update player content"
- git push

Nach dem Push baut GitHub Actions die Seite automatisch neu (GitHub Pages).

## Alternative ohne lokale Git-Tools
Du kannst Dateien auch direkt im GitHub-Webinterface bearbeiten oder hochladen (Add file -> Upload files) und dann committen.
Auch dann startet der Deploy automatisch.
