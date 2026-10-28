[Русский](README.md) · **English**

# 3D Filament Uchet — filament accounting for 3D printing

> Spools, AMS slots, projects and prints — with automatic gram deduction and
> cost calculation (filament + electricity). Offline, Windows.

## Key advantages

- **Simple installation** — one installer exe and the program is ready to use.
- **Cost per unit** — including the cost of electricity.
- **No printer integrations** — data is entered manually, simply and quickly.
- **Automatic accounting** — nothing to recalculate by hand: the database does
  all the math itself and records every spool movement.
- **Maintenance** — the program counts print hours and reminds you when the
  printer is due for service.
- **Spare spools** — if the active spool runs short, the program suggests a
  replacement for the slot.
- **Cancel a print without losses** — grams go back to their spools; if a print
  was cancelled, everything returns to where it was.
- **Offline and private** — no registration or accounts, nothing is sent to the
  internet, data stays only on your computer.
- **CSV export** — any table can be exported to a file for your own reports
  (opens in Excel).

<img width="960" height="540" alt="Img_1" src="https://github.com/user-attachments/assets/fae8735b-453a-4c14-b9d3-2805f0750080" />

## Features

**Equipment**
- Reference database: **64 printer models** and **13 filament feed systems**
  (Anycubic, Bambu Lab, Creality, Elegoo, QIDI, Flashforge, FLSUN and others);
  manufacturer and model are separate lists, feed-system compatibility follows
  official manufacturer data. Can't find your model? There are generic entries
  "Other" and "Universal AMS" (rename it to match your feed system).
- Maintenance — service types with their own intervals in print hours: "Nozzle
  inspection and cleaning", "Lead screw lubrication", "Belt check" — presets are
  ready, and you can add your own.
- Spool slots on the printer and in connected feed systems.
- Print hours, average consumption (W) per material and the price per kWh —
  electricity is included in the print cost.
- Maintenance by running hours: named service types with their own intervals (or
  your own names), marks are made with one click, overdue items are highlighted
  in the equipment card.

**Filament**
- Spool inventory: receiving (manufacturer, type, colour, weight, price),
  loading into slots, returning, scrapping.
- Remaining filament on every spool — down to hundredths of a gram, with
  inventory totals.
- Adjusting the actual weight does not distort the declared "full spool weight"
  — the price per gram stays stable.
- Spool numbers "kN" — in the "Spare spools" window and in slot tile tooltips:
  similar spools of the same colour are easy to tell apart.

**Projects and parts**
- A project is broken down into parts with colours and grams per colour;
  multi-colour parts are supported.
- Statistics for every part: good units, defective units, cost per unit.

**Prints**
- Printing by parts: grams are calculated from the project composition, and
  matching spools are selected by colour automatically; or print "by weight only".
- Arithmetic in any numeric field: add "+10" or "-10" to a number, press Enter —
  the program does the math.
- Planned weight with a breakdown ("75g × 2 = 150g"); total weight and progress
  percentage recalculate each other on the fly.
- Finishing a print early: good and defective units are accounted for, the
  printed weight per colour is recorded, and the unprinted remainder is returned
  to the spools. The weight of good units is calculated from the specification;
  defects are the remainder distributed by the average.
- Spare spools: if the active one runs short, the program suggests candidates to
  load into the slot.
- The program estimates the approximate spool-change time, so you can plan your
  day instead of guessing when it will happen.
- Shift+click on the expand triangle — expand or collapse all prints fully, down
  to spools; Ctrl+click — one print in full.

**Other**
- Filters.
- Export of tables to CSV (opens in Excel).
- Operation log.
- Hotkeys (bring the program up from any window — Ctrl+Alt+P).
- Themes: dark (default) and light (switch on the "About" tab, applied after
  restart).
- Correct operation on multiple monitors with different scaling.
- Saving and loading data: one-click backup of the database and the "History"
  log together; the "Create new database…" button starts from a clean slate;
  20 autosaves are kept.
- Running a second copy is not allowed: a message is shown and the second copy
  closes.

<img width="960" height="540" alt="Program_3DFilamentUchet_part1_shorts" src="https://github.com/user-attachments/assets/1f6ad9d6-4b8c-4898-b124-23a2251eb062" />

Video (Russian):
- Filament accounting for 3D printing — Part 1: https://vkvideo.ru/video-226164803_456239099
- Filament accounting for 3D printing — Part 2: https://vkvideo.ru/video-226164803_456239100

## How it works

The program does not sync with printers or slicers and does not control
printing. Accounting is manual: you record the key events yourself (start, pause,
resume, early finish) in the program. Filament and electricity consumption for
each job are calculated from that data. This gives precise cost control without
connecting equipment or setting up an integration.

## Installation

- Download the installer from the
  **[Releases](https://github.com/3DVopros/3DFilamentUchet/releases/latest)**
  page (file like `3DFilamentUchet-<version>-setup.exe`) and run it.
- Windows 10/11. No Python or dependencies to install.
- The installer is not digitally signed, so Windows may warn about an "unknown
  publisher" — click "More info" → "Run anyway". The program is installed into
  Program Files, user data goes to `%APPDATA%\3DFilamentUchet`.
- The program checks for new versions itself; to update, download the new
  installer and install it over the old version (data is preserved).

## Data

Everything is stored locally (SQLite, `%APPDATA%\3DFilamentUchet`). No accounts,
clouds or telemetry — the program is fully offline. Backups: the "Save and load
data" button on the "About" tab.

## License

Trial period — **45 days** with all features. After that — an activation key for
1–3 years, activation offline, no internet needed. To buy a key, use the "Buy a
license" button in the program (it opens the purchase site with your computer ID
filled in automatically) or the website
**[filamentuchet.3dvopros.ru](https://filamentuchet.3dvopros.ru)**. Terms — the
"License Agreement": it is accepted during installation — you must agree to it to
continue.

## Feedback

Questions and suggestions — the VK group "3D Vopros":
[vk.ru/3dvopros](https://vk.ru/3dvopros)
