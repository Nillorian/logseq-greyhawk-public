# GitHub Pages Setup fuer den Public Graph

## Ziel
Nach jedem Push auf `main` wird die Seite automatisch gebaut und auf GitHub Pages veroeffentlicht.

## 1. GitHub Repository verbinden

Falls noch kein Remote gesetzt ist:

```bash
git init
git branch -M main
git remote add origin https://github.com/DEIN_USER/DEIN_REPO.git
```

Falls ein Remote existiert, nur pruefen:

```bash
git remote -v
```

## 2. Dateien committen und pushen

```bash
git add .
git commit -m "Setup public vault publishing with GitHub Pages"
git push -u origin main
```

## 3. GitHub Pages im Repo aktivieren

1. GitHub Repo oeffnen.
2. Settings -> Pages.
3. Source auf `GitHub Actions` setzen.
4. Speichern.

Danach startet der Workflow automatisch bei jedem Push auf `main`.

## 4. Platzhalter in mkdocs.yml ersetzen

Datei: `mkdocs.yml`

- `YOUR_GITHUB_USERNAME` ersetzen
- `YOUR_REPOSITORY_NAME` ersetzen

Dann erneut committen und pushen.

## 5. Ergebnis

Die Seite ist danach unter folgender URL erreichbar:

`https://DEIN_USER.github.io/DEIN_REPO/`

## Troubleshooting

- Build-Fehler ansehen: GitHub -> Actions -> letzter Lauf
- Haeufige Ursache: kaputte Links oder ungueltige Markdown-Struktur
- Bei Linkproblemen zuerst `pages/index.md` und `pages/contents.md` pruefen

## Content-Regeln (Pflicht)

Vor jedem Push auf `main` die Copyright- und Freigabe-Regeln pruefen:

- `docs/PUBLIC-CONTENT-RULES.md`
