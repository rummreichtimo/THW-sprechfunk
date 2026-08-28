# THW Sprechfunk-Kompass

Interaktive Lernübersicht zu allen 10 Lernabschnitten „Sprechfunken“ der
THW-Grundausbildung (LA 9 „Verhalten im Einsatz“) sowie der Bereichsausbildung
zur ortsfesten Landfunkstelle.

Der gesamte Inhalt steckt in einer einzigen Datei: **`index.html`**.
Keine Abhängigkeiten, kein Build-Schritt, keine Datenbank — nur HTML, CSS und
etwas JavaScript. Einzige externe Ressource sind die Schriften von Google Fonts;
ohne Internetverbindung greift automatisch eine System-Schrift.

## Inhalt

| Modul | Thema | Quelle |
|------:|-------|--------|
| 01 | Auftrag & Rechtsgrundlagen | LA 01 |
| 02 | Physik & Wellenausbreitung | LA 02 |
| 03 | Sicherheit im Funkbetrieb | LA 02 |
| 04 | Analogfunk der BOS | LA 03 |
| 05 | TETRA-Digitalfunk: Grundlagen | LA 04 |
| 06 | Digitale Endgeräte | LA 05 |
| 07 | Ortsfeste Landfunkstelle | LA 10 |
| 08 | Rufgruppen im Digitalfunk | LA 06 |
| 09 | Funkrufnamen der BOS | LA 08 |
| 10 | Betriebs- & Verkehrsabwicklung | LA 07 |
| 11 | Nachrichten & Betriebsunterlagen | LA 09 |

Dazu eine Zusammenhänge-Karte, eine Gesamtzusammenfassung und ein
Prüfungs-Schnellcheck mit 22 Fragen.

## Als GitHub Page veröffentlichen

Es gibt zwei Wege. **Weg A** ist der einfachere.

### Weg A — direkt aus dem Branch (ohne Actions)

1. Im Repository auf **Settings** → in der linken Spalte auf **Pages**.
2. Bei **Source** → **Deploy from a branch** auswählen.
3. Bei **Branch** den Branch wählen, auf dem `index.html` liegt, und als Ordner
   **`/ (root)`**. Dann **Save**.
4. Nach etwa einer Minute steht die Adresse oben auf derselben Seite:
   `https://rummreichtimo.github.io/THW-sprechfunk/`

Die Datei `.nojekyll` sorgt dafür, dass GitHub die Seite unverändert ausliefert
und nicht durch den Jekyll-Generator schickt.

### Weg B — über GitHub Actions

In `.github/workflows/pages.yml` liegt ein fertiger Workflow.

1. **Settings** → **Pages** → bei **Source** → **GitHub Actions** auswählen.
2. Der Workflow läuft bei jedem Push auf `main` bzw. auf den Entwicklungsbranch
   und lässt sich unter **Actions** → *Deploy to GitHub Pages* → **Run workflow**
   auch von Hand starten.

### Tipp: Branch umbenennen

Der Standardbranch heißt aktuell `claude/interactive-learning-overview-nvye2m`.
Unter **Settings** → **General** → **Default branch** lässt er sich mit dem
Stift-Symbol in `main` umbenennen — das macht beide Wege oben übersichtlicher.
Der Workflow ist bereits auf beide Namen eingestellt.

## Lokal ansehen

`index.html` einfach im Browser öffnen — oder für saubere Adressen:

```bash
python3 -m http.server 8000
# danach http://localhost:8000 aufrufen
```

## Hinweise zum Inhalt

Alle Inhalte stammen ausschließlich aus den zehn bereitgestellten
THW-Präsentationen (241 Folien) — ausgewertet wurden Folientexte, die Inhalte
der Folien-Grafiken und die Referentennotizen. Es wurde nichts ergänzt oder
erfunden. Stellen, an denen die Unterlagen selbst unvollständig oder
uneinheitlich sind, sind im Text gekennzeichnet.

Diese Lernübersicht ersetzt weder die Ausbildung noch die geltenden
Dienstvorschriften (PDV/DV 810.3, THW-DV 1-820, NBHB THW).
