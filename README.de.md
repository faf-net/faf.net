# faf.net — Amiga Workbench 1.3 im Browser

[English](README.md) · **Deutsch**

Wer https://faf.net aufruft, landet auf einem nachgebauten **Amiga-Workbench-1.3-Desktop**:
AmigaDOS-Boot, Fenster, Schubladen, Menüs, Topaz-Schrift, Originalpalette — alles in einer
einzigen HTML-Datei, gezeichnet auf einem Canvas mit echtem Hires-Raster (Pixel doppelt so
hoch wie breit). Keine Frameworks, kein Build-Schritt, keine Tracker.

## Dateien

| Datei | Inhalt |
|---|---|
| `index.html` | die Workbench (HTML/CSS/JS inline, Topaz-8 eingebettet) |
| `wopr.html` | WOPR-Terminal aus *WarGames* (1983) — grüner CRT-Look, Tic-Tac-Toe gegen eine unschlagbare KI |
| `kickstart13.png` | die Workbench-1.3-Diskette mit Hand, im Fenster „Kickstart 1.3“ |
| `pgpkey.asc` | der öffentliche OpenPGP-Schlüssel (auch bei keys.openpgp.org und per WKD) |
| `v1/` | erster Stand der Workbench (Sicherung) |

**Deployment:** `index.html`, `wopr.html`, `kickstart13.png` und `pgpkey.asc` ins Web-Root, fertig.

## Was drin ist

```
 Desktop   faf.net · RAM DISK · DF1:NDOS · WOPR
 faf.net   About · GitHub · Workbench
           System · Utilities · Games
           PGP Key · Trashcan
 Trashcan  Windows95.exe
 System    Kickstart · Shell · Clock · Prefs
 Utilities X-Copy · VirusX · SysInfo · SCA-Virus · ByteBandit
 Games     Caves
```

- **Workbench:** Fenster ziehen, skalieren, schließen, Tiefe; Icons auswählen (Komplementfarben,
  Schubladen ziehen sich auf) und per Doppelklick öffnen; Rechtsklick-Menü (Touch: Titelleiste
  antippen) mit Clean Up, Version u. a.; Amiga-Mauszeiger samt „Zz“-Wolke.
- **Palette:** Icon „Workbench“ schaltet die vier Farbregister zwischen Original 1.3 und dem
  **Workbench Design 1.0** um — ein persönliches Design-System in warmen, gedämpften Farben mit
  einem einzigen Akzent in Bernstein, benannt nach dem Betriebssystem des Amiga
  ([faf-net/workbench](https://github.com/faf-net/workbench)).
- **Speicher wie auf einem A500 mit 512K Chip-RAM:** Fenster kosten Speicher; wird es knapp,
  kommt „Not enough memory“, beim dritten Versuch in Folge eine Guru Meditation.
- **AmigaShell:** `help`, `dir`, `info`, `avail`, `date`, `type about`, `version`, `xcopy`,
  `virusx`, `sysinfo`, `caves`, `reboot`, `sound off|on`, `guru` …
- **Clock** mit Rauten, Rautenzeigern und Datum; **Kickstart**-Bild im Fenster.
- **X-Copy:** Nachbau des Original-Bildschirms (Cachet 1988) mit Modi, START/END,
  Laufwerken und Spurrastern; COPY nach DF1: macht aus der NDOS-Diskette eine Kopie.
- **Viren (harmlos, nur per Doppelklick):** **SCA** (1987) mit Originalmeldung; **Byte Bandit**
  (1988) — Bildschirm wird dunkel, Tastatur „tot“, Bootblock-String glimmt auf. **VirusX**
  findet und entfernt beide.
- **DF1:NDOS** → Requester „Not a DOS disk“.
- **SysInfo:** ein A500 neben dem Rechner des Besuchers (nichts verlässt den Browser).
- **DIAMOND CAVES:** Höhlenspiel im Stil von Boulder Dash — graben, Diamanten, fallende
  Felsen, Glühwürmchen und Schmetterlinge, erzeugte Höhlen mit steigender Schwierigkeit,
  Highscore im Browser. Pfeiltasten/WASD, Leertaste, R, Esc; am Handy Wischen oder Steuerkreuz.
- **WOPR** auf dem Desktop führt zum WarGames-Terminal.
- **Windows95.exe** liegt im Trashcan. Es braucht einen richtigen Computer; wer es trotzdem
  startet, bekommt auf einem eigenen Screen den Bluescreen. Eine Taste führt zurück,
  Strg+Alt+Entf startet den Amiga neu.
- **Prefs** stellt die vier Farbregister mit R/G/B-Reglern ein, 16 Stufen je Farbe wie beim A500
  (4.096 Farben); Use gilt für den Besuch, Save dauerhaft, Reset holt die Palette zurück.
- **Info** (Workbench-Menü, rechte Maustaste) zeigt Name, Typ, Blöcke, Bytes und Kommentar des
  gewählten Icons.
- **Screens** lassen sich wie beim echten Amiga an der Titelleiste herunterziehen; die
  Tiefen-Gadgets und Alt+M wechseln sie.
- **PGP Key:** OpenPGP-Schlüssel (ed25519/cv25519, Fingerabdruck `1E27 72BA 59E0 791E 146C CB23 5F8D 266C 7127 8827`)
  mit Mail, Download und einem Schlüsselfenster mit Copy. Die E-Mail-Adresse steht nirgends als Text
  im Quelltext — sie wird erst zur Laufzeit zusammengesetzt und nur auf den Canvas gezeichnet.

## Herkunft und Rechte

- **Topaz a500** (Kickstart 1.x) als Bitmap von dMG/t!s^dS!, rewtnull/amigafonts,
  GPL mit Font-Ausnahme; Topaz © Amiga Inc.
- Icons, Fenster, X-Copy-Bildschirm, Spielgrafik und Töne sind selbst gezeichnet bzw. per
  WebAudio erzeugt. X-Copy, SCA, Byte Bandit, VirusX und Boulder Dash sind Hommagen;
  deren Namen und Marken gehören den jeweiligen Rechteinhabern.
- Beschreibung der Viren nach der Amiga Virus Encyclopedia (vht-dk.dk).
- Disk-, Schubladen- und Trashcan-Icons sowie die Fenster-Gadgets folgen Workbench 1.3 Pixel für
  Pixel, ausgemessen an [TAWS](https://www.taws.ch/WB.html) von Michael Rupp; die Grafiken sind © Commodore-Amiga.
- Der Bluescreen ist eine Parodie mit eigenem Text; Windows ist eine Marke von Microsoft.
- `kickstart13.png` zeigt die Kickstart-1.3-Grafik (© Commodore-Amiga) als Zitat.

## Lizenz

Eigener Code und eigene Grafik: **MIT** (siehe `LICENSE`, Fremdanteile in `NOTICE`). Ausgenommen sind die Topaz-Schrift
(GPL mit Font-Ausnahme) und `kickstart13.png` (© Commodore-Amiga).
