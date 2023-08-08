# SOCO Webseite

## Seite bearbeiten

* `md`-Datei unter `docs` heraussuchen
* Änderungen machen
* Git Commit / Änderungen als Commit über Github-Webseite speichern
* GitHub Actions kümmern sich um die Veröffentlichung

## Seite Hinzufügen

* Datei `neue-seite.md` unter `docs` hinzufügen
* In `mkdocs.yml` unter `nav` die Seite `neue-seite.md` registrieren

## Lokal entwickeln / testen

Man kann das ganze auch lokal testen

### Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### Lokal testen

```bash
source .venv/bin/activate
mkdocs serve
```

Dann http://127.0.0.1:8000/ im Browser öffnen
