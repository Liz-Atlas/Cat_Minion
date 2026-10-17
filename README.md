# Cat_Minion
Cat logik.
# 🐾 Cat Minion

*Einmal falsch geatmet, schon enterbt.*

Ein kleines Browser-Spiel: 24 Stunden als Personal zweier Senioren-Katzen.
**Pinkey** (die autonome Monarchin) und **Puma** (der Klettverschluss mit Reißzähnen).
Sechs Alltagssituationen, drei Antworten, und ein Minion-Report, der erklärt, warum deine menschliche Logik gerade an der Katzen-Biologie zerschellt ist.

Zwei Modi:
- **🕒 Ein Tag als Minion** – sechs echte Szenen mit Pinkey und Puma, drei Status-Balken, Boss-Level um Mitternacht.
- **📚 Minion-Prüfung** – allgemeines Katzenwissen: 10 zufällige Fragen aus einem Pool von 18, jede Runde neu gemischt.

Entstanden als Fun-Projekt zwischen Mensch und KI.

## Spielen

Einfach `index.html` im Browser öffnen. Keine Installation, keine Abhängigkeiten.

## GitHub Pages

1. Repo anlegen, `index.html` und `README.md` hochladen
2. **Settings → Pages → Source:** `Deploy from a branch`, Branch `main`, Ordner `/ (root)`
3. Nach einer Minute läuft das Spiel unter `https://<username>.github.io/<repo>/`

## Eigene Bilder

Lege einen Ordner `img/` an und speichere die Bilder unter diesen Namen:

| Datei | Wofür |
|---|---|
| `img/pfote.jpg` | Belohnung – die heilige Flausch-Pfote |
| `img/blick.jpg` | Strafe Pinkey – der Blick vom Holzstuhl |
| `img/pantoffel.jpg` | Strafe Puma – Tatort Badezimmer |
| `img/handschuh.jpg` | Strafe Tierarzt – der zerfetzte Handschuh |

Fehlt ein Bild, zeigt das Spiel automatisch ein Emoji.

## Neue Level

Alle Level stehen im `LEVELS`-Array in `index.html`. Jede Option hat:
`t` (Antworttext), `type` (`win` / `ok` / `fail`), `img` oder `emo`, `d` (Punkte für `pinkey`, `puma`, `slipper`), sowie `thought`, `cat` und `fact` für den Minion-Report.

## Neue Quizfragen

Im `QUIZ`-Array: `q` (Frage), `opts` (drei Antworten, die richtige mit `ok:true`), `cat` (Katzen-Kommentar) und `fact`. Die Reihenfolge der Antworten wird automatisch gemischt.
