# faf.net — Amiga Workbench 1.3 in the browser

**English** · [Deutsch](README.de.md)

Visit https://faf.net and you land on a recreated **Amiga Workbench 1.3 desktop**:
AmigaDOS boot, windows, drawers, menus, the Topaz font and the original palette — all in a
single HTML file, drawn on a canvas with a true hires raster (pixels twice as tall as they are
wide). No frameworks, no build step, no trackers.

## Files

| File | Contents |
|---|---|
| `index.html` | the Workbench (HTML/CSS/JS inline, Topaz 8 embedded) |
| `wopr.html` | the WOPR terminal from *WarGames* (1983) — green CRT look, tic-tac-toe against an unbeatable AI |
| `kickstart13.png` | the Workbench 1.3 disk in hand, shown in the "Kickstart 1.3" window |
| `pgpkey.asc` | the OpenPGP public key (also on keys.openpgp.org and via WKD) |
| `v1/` | the first version of the Workbench (backup) |

**Deployment:** copy `index.html`, `wopr.html`, `kickstart13.png` and `pgpkey.asc` to the web root. Done.

## What's inside

```
 Desktop   faf.net · RAM DISK · DF1:NDOS · WOPR
 faf.net   About · GitHub · Workbench
           System · Utilities · Games
           PGP Key · Trashcan
 System    Kickstart · Shell · Clock
 Utilities X-Copy · VirusX · SysInfo · SCA-Virus · ByteBandit
 Games     Caves
```

- **Workbench:** drag, resize, close and depth-arrange windows; select icons (complement
  colours, drawers slide open) and open them with a double-click; right-click menu (touch: tap
  the title bar) with Clean Up, Version and more; the Amiga pointer including the "Zz" cloud.
- **Palette:** the "Workbench" icon switches the four colour registers between the original
  1.3 colours and **Workbench Design 1.0** — a personal design system in warm, muted colours
  with a single amber accent, named after the Amiga's operating system
  ([faf-net/workbench](https://github.com/faf-net/workbench)).
- **Memory like an A500 with 512K chip RAM:** windows cost memory; when it runs low you get
  "Not enough memory", and on the third attempt in a row a Guru Meditation.
- **AmigaShell:** `help`, `dir`, `info`, `avail`, `date`, `type about`, `version`, `xcopy`,
  `virusx`, `sysinfo`, `caves`, `reboot`, `sound off|on`, `guru` …
- **Clock** with diamond markers, diamond-shaped hands and the date; the **Kickstart** picture
  in a window.
- **X-Copy:** a recreation of the original screen (Cachet, 1988) with modes, START/END, drives
  and track grids; COPY to DF1: turns the NDOS disk into a copy.
- **Viruses (harmless, double-click only):** **SCA** (1987) with its original message;
  **Byte Bandit** (1988) — the screen goes dark, the keyboard "dies", the bootblock string
  glows up. **VirusX** finds and removes both.
- **DF1:NDOS** → the "Not a DOS disk" requester.
- **SysInfo:** an A500 next to the visitor's machine (nothing leaves the browser).
- **DIAMOND CAVES:** a cave game in the spirit of Boulder Dash — digging, diamonds, falling
  boulders, fireflies and butterflies, generated caves of rising difficulty, high scores kept
  in the browser. Arrow keys/WASD, space, R, Esc; on phones swipe or use the on-screen pad.
- **WOPR** on the desktop leads to the WarGames terminal.
- **PGP Key:** OpenPGP key (ed25519/cv25519, fingerprint `1E27 72BA 59E0 791E 146C CB23 5F8D 266C 7127 8827`)
  with Mail, Download and a key window with Copy. The e-mail address never appears as text in
  the page source — it is assembled at run time and only drawn onto the canvas.

## Credits and rights

- **Topaz a500** (Kickstart 1.x) bitmap by dMG/t!s^dS!, rewtnull/amigafonts, GPL with font
  exception; Topaz © Amiga Inc.
- Icons, windows, the X-Copy screen, game graphics and sounds are hand-drawn or generated with
  WebAudio. X-Copy, SCA, Byte Bandit, VirusX and Boulder Dash are homages; their names and
  trademarks belong to their respective owners.
- Virus behaviour as described by the Amiga Virus Encyclopedia (vht-dk.dk).
- `kickstart13.png` shows the Kickstart 1.3 artwork (© Commodore-Amiga) as a quotation.

## License

Own code and own graphics: **MIT** (see `LICENSE`, third-party parts in `NOTICE`). Excluded are
the Topaz font (GPL with font exception) and `kickstart13.png` (© Commodore-Amiga).
