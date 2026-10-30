# Reisetagebuch

Ein Reiseblog im Kritzel-Tagebuch-Stil für GitHub Pages.

## Was wo liegt

| Datei / Ordner | Inhalt |
|---|---|
| `index.html` | Die Webseite (alles auf einer Seite) |
| `style.css` | Das Aussehen: Farben, Schriften, Fotos. Farben und Schriften stehen ganz oben bei `:root` |
| `_config.yml` | Titel und Untertitel der Seite |
| `_posts/` | Die Einträge, eine Datei pro Eintrag |
| `bilder/` | Alle Fotos |
| `VORLAGE.md` | Vorlage für neue Einträge |
| `ANLEITUNG.md` | Schritt-für-Schritt-Anleitung zum Schreiben |

Die Beispiel-Einträge in `_posts/` und `bilder/beispiel-lyon.svg` können gelöscht werden.

## Regeln für Dateinamen

Für alle Dateinamen gilt: **nur Kleinbuchstaben, Zahlen und Bindestriche.** Keine Leerzeichen, keine ä/ö/ü, kein ß.

| statt | besser |
|---|---|
| `Strand Tag.jpg` | `strand-tag.jpg` |
| `Zürich.jpg` | `zuerich.jpg` |
| `IMG_4711.JPG` | `img-4711.jpg` |

### Einträge (Ordner `_posts`)

```
JJJJ-MM-TT-titel.md
```

- Beispiel: `2026-07-12-strand-tag.md`
- Vorne immer das Datum: Jahr-Monat-Tag, mit Nullen (`07`, nicht `7`).
- Das Datum bestimmt die Reihenfolge. Der neueste Eintrag steht zuoberst.
- Ein Datum in der Zukunft wird nicht angezeigt.
- Hinten immer `.md`.
- Die Datei muss mit dem Kopf zwischen zwei `---` Linien beginnen (siehe `VORLAGE.md`).

### Fotos (Ordner `bilder`)

Es gibt zwei Arten von Fotos. Welche Art es wird, entscheidet allein der Dateiname.

| Art | Dateiname | Wie es aussieht |
|---|---|---|
| **Normales Foto** | ohne das Wort `seite`, z. B. `tag3-kirche.jpg` | Kleines, schräges Sofortbild mit Klebeband |
| **Fotografierte Tagebuchseite** | mit `seite` im Namen, z. B. `tag3-seite.jpg` | Über die ganze Breite, damit die Schrift lesbar ist |

Empfehlung: Fotos immer mit dem Tag beginnen lassen, dann findet man sie leicht wieder.

```
tag3-seite.jpg      Tagebuchseite von Tag 3
tag3-seite-2.jpg    zweite Seite von Tag 3
tag3-kirche.jpg     normales Foto
```

Achtung: Jedes Foto mit `seite` irgendwo im Namen wird gross angezeigt, also auch `rueckseite.jpg`. Solche Namen vermeiden.

Ins Eintrag-File kommt ein Foto so:

```
![Bildunterschrift](bilder/tag3-seite.jpg)
```

Der Name muss genau stimmen, auch die Endung: `.jpg` ist nicht dasselbe wie `.JPG` oder `.jpeg`.

### Fotogrösse

- Tagebuchseiten: etwa **1500 Pixel** breit, damit die Schrift lesbar bleibt.
- Normale Fotos: etwa **1000 Pixel** breit reichen.
- Handyfotos in voller Grösse machen die Seite langsam.

## Veröffentlichen

Settings → Pages → Source „Deploy from a branch“ → Branch `main`, Ordner `/ (root)` → Save.

Nach jeder Änderung dauert es 1–2 Minuten, bis sie online ist. Den Stand sieht man im Reiter **Actions**.
