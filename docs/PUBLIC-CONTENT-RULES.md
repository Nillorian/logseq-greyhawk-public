# Regeln für öffentliche Inhalte (Copyright)

Diese Regeln gelten für alle Inhalte im Public-Repo und auf GitHub Pages.

## Grundsatz

Nur Inhalte veröffentlichen, für die wir die nötigen Rechte haben.

Zulässig sind:
- Eigene Texte, Bilder, Karten und Dateien.
- Inhalte mit klarer, passender Lizenz (z. B. CC BY, CC BY-SA, Public Domain).
- Stock-Material mit gültiger Lizenz oder Kaufnachweis.

Nicht zulässig sind:
- Übernommene Texte/Bilder aus Büchern, PDFs, Websites, Wikis oder Foren ohne Erlaubnis.
- Inhalte mit unklarer Herkunft oder unklarer Lizenz.
- "Leicht umgeschriebene" fremde Texte ohne Nutzungsrecht.

## Wichtiger Hinweis zu GitHub Pages

Bei einem Public-Repository ist nicht nur die Website öffentlich, sondern auch das gesamte Repository.
Damit sind auch unverlinkte Dateien, Assets und Commit-Historie potenziell einsehbar.

## Pflicht für externe Assets

Für jedes externe Asset muss ein Nachweis vorliegen:
- Titel
- Urheber
- Quelle (URL)
- Lizenz
- Abrufdatum
- Geplante Nutzung im Repo

Wenn ein Nachweis fehlt, wird das Asset nicht veröffentlicht.

## Freigabe-Check vor jedem Push auf main

1. Gibt es fremde Inhalte ohne klare Lizenz? Dann entfernen oder ersetzen.
2. Sind alle externen Assets mit Quelle und Lizenz dokumentiert? Sonst nicht pushen.
3. Enthalten Texte direkte Übernahmen aus fremden Werken? Dann umarbeiten oder entfernen.
4. Enthalten Seiten DM-only oder interne Notizen? Dann entfernen.
5. Lokale/temporäre Dateien (z. B. .venv) sind nicht im Repo versioniert.

## Seitenformat für GitHub Pages

Für öffentliche Seiten gilt ein MkDocs-kompatibles Markdown-Format:
- Keine proprietäre Property-Syntax in Seiteninhalten verwenden (z. B. type::, tags::, status::).
- Metadaten direkt unter der H1 als normale Markdown-Liste pflegen.
- Tags als Klartext im Metadatenblock und optional zusätzlich in einem eigenen Abschnitt aufführen.
- Inhalte in üblichen Markdown-Abschnitten mit Überschriften strukturieren.
- Deutschsprachige Seiten mit korrekter Rechtschreibung inklusive Umlauten und ß pflegen.

Referenz für Vorlagen und Feldnamen:
- pages/Templates.md

## Incident-Regel

Wenn problematische Inhalte bereits gepusht wurden:
1. Datei sofort aus dem aktuellen Stand entfernen.
2. Inhalte aus der Git-Historie entfernen (History-Rewrite), damit sie nicht weiter abrufbar sind.
3. Danach neu pushen und Pages-Deploy erneut ausführen.

## Verantwortlichkeit

Bei Unsicherheit gilt: Nicht veröffentlichen, bis Rechte eindeutig geklärt sind.

---

Diese Datei ist eine Projektregel und keine Rechtsberatung.
