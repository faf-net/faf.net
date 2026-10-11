# faf.net — WOPR-Landingpage

Private Spaß-Landingpage: Wer https://faf.net aufruft, landet in einem
nachgebauten WOPR-Terminal aus *WarGames – Kriegsspiele* (1983) — grüner
CRT-Look, 300-Baud-Boot-Sequenz, interaktives Terminal, Tic-Tac-Toe gegen
eine unschlagbare KI (Minimax). Verrät bewusst nichts Persönliches.

- **Einzige Datei:** `index.html` (~22,5 KB) — HTML/CSS/JS vollständig
  inline, keine Abhängigkeiten, kein Build-Schritt.
- **Deployment:** Diese Datei unverändert ins Web-Root hochladen, fertig.
- **Hosting:** statisches Webhosting, keine Server-Logik.
- **Stand geprüft:** 13.08.2026 — lokale Kopie hier ist byte-identisch mit
  der Live-Version unter https://faf.net.


## Entwurf 11.10.2026 — Workbench 1.3

- **`index.html`** (seit 11.10.2026 die Workbench, vorher `workbench.html`; ~39 KB, eine Datei, keine Abhängigkeiten): faf.net als
  Amiga-Workbench-1.3-Desktop. Canvas mit echtem Hires-Raster (Pixel doppelt so
  hoch wie breit), Topaz-8-Font aus Kickstart 1.x eingebettet, Originalpalette
  (#0055AA / #FFFFFF / #000022 / #FF8800). Boot-CLI → Workbench, Fenster
  ziehen/skalieren/schließen/Tiefe, Icons wählen (Komplementfarben) und per
  Doppelklick öffnen, Rechtsklick-Menü (Touch: Tipp auf Titelleiste), Clock,
  AmigaShell (`help`, `dir`, `info`, `avail`, `type about`, `github`, `guru` …).
  GitHub-Icon (Octocat, selbst gezeichnet) öffnet https://github.com/faf-net im neuen Tab.
  Icon „Workbench“ (Farbregister wie in Preferences) schaltet die vier Register
  zwischen Original 1.3 und dem Workbench Design 1.0 (github.com/faf-net/workbench,
  dunkel: grund #1a1918 · schrift #e9e3d8 · linie #3a3634 · bernstein #cc9166) um;
  Wahl bleibt per localStorage im Browser des Besuchers. Shell: `palette`.
- **`wopr.html`** = unveränderte bisherige WOPR-`index.html` (byte-gleich geprüft); das WOPR-Icon
  auf der Workbench springt dorthin.
- **Lokal umgestellt, noch nicht live.** Zum Live-Schalten `index.html` und
  `wopr.html` ins Web-Root hochladen.
- `_quellen/` — Topaz-Rohdaten (rewtnull/amigafonts, GPL-FE), nicht hochladen.
