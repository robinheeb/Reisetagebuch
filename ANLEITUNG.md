# So schreibst du einen neuen Eintrag

Alles geht direkt auf github.com im Browser. Am besten am Computer oder Tablet.

## 1. Neuen Eintrag anlegen

1. Öffne das Repository auf github.com und klick auf den Ordner **`_posts`**.
2. Klick oben rechts auf **Add file** → **Create new file**.
3. Gib der Datei einen Namen nach diesem Muster:

   `2026-07-12-titel-ohne-leerzeichen.md`

   - Zuerst das Datum: Jahr-Monat-Tag
   - dann ein kurzer Titel, Wörter mit Bindestrichen verbunden
   - am Schluss **`.md`**
   - keine Leerzeichen, keine ä/ö/ü (also `strand-tag` statt `Strand Tag`)
4. Öffne die Datei **`VORLAGE.md`** in einem zweiten Tab, kopiere alles und füge es in deine neue Datei ein.
5. Ändere die Überschrift, den Ort und den Text.
6. Klick oben rechts auf **Commit changes…** und dann nochmals auf **Commit changes**.

Nach 1–2 Minuten ist der Eintrag auf der Webseite. Neuester Eintrag steht immer zuoberst.

## 2. Was die Zeilen oben bedeuten

Der Teil zwischen den zwei `---` Linien sind die Infos zum Eintrag:

| Zeile | Was du einträgst |
|---|---|
| `title:` | Die Überschrift, in Anführungszeichen |
| `ort:` | Wo du warst. Steht dann auf der Karte |
| `koordinaten:` | Wo genau der Ort ist, zum Beispiel `41.3874, 2.1686` (siehe unten). Darfst du auch weglassen, dann kommt der Ort nicht auf die Karte |
| `laune:` | Wie war der Tag? Eine Zahl von 1 bis 10, zum Beispiel `laune: 8`. Auf der Seite erscheinen dann 8 goldene und 2 graue Sterne |

**Koordinaten finden:** In Google Maps mit der rechten Maustaste (am Handy: lange drücken) auf den Ort tippen. Oben erscheinen zwei Zahlen, zum Beispiel `41.3874, 2.1686`. Anklicken kopiert sie. Dann einfach hinter `koordinaten:` einfügen:

`koordinaten: 41.3874, 2.1686`

Wichtig: Die beiden Zahlen müssen mit einem Komma getrennt sein, und in den Zahlen selbst steht ein Punkt, kein Komma.

## 3. Fotos hochladen

1. Öffne den Ordner **`bilder`**.
2. Klick auf **Add file** → **Upload files** und zieh deine Fotos hinein.
3. Unten auf **Commit changes** klicken.
4. Im Eintrag schreibst du dann an die Stelle, wo das Foto hin soll:

   `![Das ist die Bildunterschrift](bilder/name-vom-foto.jpg)`

**Tagebuchseiten:** Hast du eine Seite aus deinem Heft fotografiert, muss im Dateinamen das Wort `seite` vorkommen, zum Beispiel `tag3-seite.jpg`. Dann wird sie gross angezeigt, damit man deine Schrift lesen kann. Alle anderen Fotos werden kleine Sofortbilder.

**Achtung:**
- Der Name muss genau stimmen, auch Gross- und Kleinschreibung. `Strand.JPG` ist nicht dasselbe wie `strand.jpg`.
- Fotos vorher umbenennen: ohne Leerzeichen, ohne ä/ö/ü.
- Handyfotos sind riesig. Verkleinere sie vorher (z. B. beim Teilen „mittlere Grösse“ wählen), sonst lädt die Seite ewig.

## 4. Eintrag ändern oder löschen

Datei im Ordner `_posts` anklicken, dann oben rechts auf den **Stift** (ändern) oder auf **…** → **Delete file** (löschen). Danach wieder **Commit changes**.

## 5. Was nicht ins Tagebuch gehört

Die Seite kann jeder sehen. Deshalb: kein Nachname, keine Adresse, keine Schule, keine Telefonnummern und keine Fotos von anderen Leuten ohne zu fragen. Und erst schreiben, wo ihr wart, nicht wo ihr gerade seid.

## Wenn etwas nicht klappt

- **Eintrag erscheint nicht?** Stimmt der Dateiname? Datum vorne, `.md` hinten? Ein Datum in der Zukunft wird nicht angezeigt.
- **Seite zeigt einen Fehler oder ändert sich nicht?** Im Repository auf den Reiter **Actions** schauen. Ein rotes Kreuz heisst: Irgendwo ist ein Tippfehler, oft fehlt bei `title:` ein Anführungszeichen.
- **Foto fehlt?** Dateiname im Eintrag und im Ordner `bilder` vergleichen.
