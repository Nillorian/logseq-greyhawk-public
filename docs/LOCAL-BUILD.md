# Lokal bauen und Build-Fehler pruefen

Diese Schritte helfen dir, die Seite lokal zu bauen und Fehler frueh zu sehen (bevor du pushst).

## 1) In das Repoverzeichnis wechseln

## 2) Virtuelle Umgebung anlegen (einmalig)

```bash
python3 -m venv .venv
source .venv/bin/activate
```

## 3) Abhaengigkeiten installieren

```bash
pip install -r requirements.txt
```

## 4) Strikten Build ausfuehren (empfohlen)

```bash
mkdocs build --strict
```

Was passiert:
- Die statische Seite wird nach `site/` gebaut.
- Warnungen (z. B. defekte Links) werden als Fehler behandelt.
- Exit Code ungleich `0` bedeutet: Build ist fehlgeschlagen.

## 5) Optional: Lokal im Browser testen

```bash
mkdocs serve
```

Dann im Browser oeffnen: `http://127.0.0.1:8000/`

## 6) Schneller Pre-Push-Check

```bash
source .venv/bin/activate && mkdocs build --strict
```

Wenn dieser Befehl sauber durchlaeuft, sind die haeufigsten Build-/Link-Probleme lokal bereits abgefangen.

## Typische Fehlerquellen

- Datei in `pages/` umbenannt, aber Link nicht angepasst.
- Markdown-Datei fehlt in der Navigation (`mkdocs.yml`), obwohl sie verlinkt wird.
- Falsche relative Pfade bei Assets unter `pages/assets/`.
