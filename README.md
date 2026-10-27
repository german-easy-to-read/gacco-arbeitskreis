# Arbeitskreis German Accessible Communication (GACCO)

Website des Arbeitskreises, gebaut mit [Jekyll](https://jekyllrb.com/) und dem
Remote-Theme [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes),
gehostet über GitHub Pages.

## Struktur

| Pfad | Inhalt |
| ---- | ------ |
| `index.md` | Landingpage – hier stehen alle Inhalte zum Arbeitskreis |
| `_pages/news.md` | Übersichtsseite aller Newsbeiträge (`/news/`) |
| `_pages/404.md` | Fehlerseite |
| `_posts/` | Die einzelnen Newsbeiträge (Deutsch) |
| `en/` | Englische Version: `index.md`, `news.md`, `_posts/` (unter `/en/`) |
| `_data/navigation.yml` | Einträge der Hauptnavigation, je Sprache |
| `_data/i18n.yml` | Sprachen und Startseiten für den Sprachumschalter |
| `_includes/`, `_layouts/` | Angepasste Theme-Dateien (Navigation mit Sprachumschalter, sprachgefilterte Newsliste) |
| `assets/css/main.scss` | Eigene Styles (Breite des Textbereichs, Sprachumschalter) |
| `_config.yml` | Titel, Beschreibung, Theme-Einstellungen |
| `assets/images/` | Bilder (Logo, Fotos) |

## News hinzufügen

Eine neue Datei in `_posts/` anlegen, benannt nach dem Schema
`JJJJ-MM-TT-kurztitel.md`:

```markdown
---
title: "Titel der Meldung"
date: 2026-11-15 10:00:00 +0100
excerpt: "Ein bis zwei Sätze für die Übersicht."
---

Der Text der Meldung.
```

## Zweisprachigkeit (Deutsch/Englisch)

Deutsch ist die Standardsprache und liegt unter `/`, Englisch unter `/en/`.
Alles im Ordner `en/` wird automatisch als Englisch markiert.

Damit der Sprachumschalter oben rechts direkt auf die Übersetzung einer Seite
springt, bekommen beide Fassungen im Front Matter denselben `ref`-Wert, z. B.
`ref: website-online`. Fehlt eine Übersetzung, führt der Umschalter auf die
Startseite der anderen Sprache.

Englische News kommen nach `en/_posts/` (gleiches Dateischema wie oben) und
erscheinen unter `/en/news/`.

Beim Push nach `master` baut GitHub Pages die Seite automatisch neu.

## Lokal ansehen

```bash
bundle install
bundle exec jekyll serve
```

Danach läuft die Seite unter <http://localhost:4000>.

## Vor dem Livegang

- In `_config.yml` `url` und – bei einer Project Page – `baseurl` eintragen.
- E-Mail-Adresse in `_config.yml` (`email`, Footer-Link) ergänzen.
- Platzhaltertexte in `index.md` ersetzen und den Beispielbeitrag in `_posts/`
  löschen.
