# Universal Electronics Box

Modular DIN-rail electronics enclosure for Millennium CNC builds—designed to pair with [Milo V2 / Miley V2](https://github.com/MillenniumMachines/Milo-V2.0).

**Repository:** [github.com/MillenniumMachines/Universal-Electronics-Box](https://github.com/MillenniumMachines/Universal-Electronics-Box)

This repository contains **STLs**, **panel DXFs**, **master CAD**, the **bill of materials** spreadsheet, **print list**, and the **wiring reference PDF**. Human-readable BOM, print settings, and part tables live on the [UEB section of the Millennium Machines documentation site](https://millenniummachines.github.io/docs/ueb/); see also the [main documentation hub](https://millenniummachines.github.io/docs/) for other Millennium projects.

## Documentation

| Topic | Location |
| --- | --- |
| All Millennium Machines guides | [Documentation hub](https://millenniummachines.github.io/docs/) |
| Overview, safety, repo layout | [UEB docs — Overview](https://millenniummachines.github.io/docs/ueb/) |
| Bill of materials and contactor options | [Sourcing guide](https://millenniummachines.github.io/docs/ueb/bom/sourcing_guide/) |
| Print profiles and printed parts | [Printing guide](https://millenniummachines.github.io/docs/ueb/printing/print_guide/) |
| Mains, E-stop, PSU, and signal wiring | [Millennium Universal CNC wiring .pdf](Millennium%20Universal%20CNC%20wiring%20.pdf) |
| Milo mechanical build, RRF, pre-flight | [MiloV2-Manual.pdf](https://github.com/MillenniumMachines/Milo-V2.0/blob/main/Manual/MiloV2-Manual.pdf) |

Source spreadsheets in this repo (also reflected on the docs site):

- `Electronics Cabinet BOM.xlsx`
- `Milennium Universal Electronics box Print List.xlsx`

## Repository layout

```
CAD/          Master assembly STEP
DXFs/         Top/bottom and side panel outlines
STLs/
  Panels/     Covers, clips, handles, keystone blanks
  Mounts/     DIN-rail mounts (Scylla, LRS-350 PSU)
  Cable channels/   Lids and trays for wire routing
              TPU-Foot-x4-A.stl (optional feet)
```

## Printing quick reference

Use **0.2 mm** layers and a **0.4 mm** nozzle unless you are experimenting. Profile codes in filenames match the print list:

| Code | Use |
| --- | --- |
| **S** | Structural — 45% infill, 6 walls |
| **SS** | Semi-structural — 25% infill, 4 walls |
| **A** | Aesthetic — 20% infill, 3 walls |

- **`[a]`** prefix — accent filament
- **`x#`** suffix — quantity required (e.g. `x4` → four copies)
- **`Voron-Inserts`** in the filename — print the variant that matches your heat-set inserts (Voron vs CNC-Kitchen)

See the [printing guide](https://millenniummachines.github.io/docs/ueb/printing/print_guide/) for the full part list.

## Wiring

The wiring PDF is titled **V2 / V1.6 wiring reference**. It covers mains inlet, breaker, contactor, 24 V distribution, E-stop, and machine interconnect—follow it together with your local electrical code.

> **Warning:** This enclosure operates at **mains voltage**. Use a suitable E-stop, correct wire gauges for your region, and qualified help if you are unsure. Do not energize the cabinet until wiring has been checked.

## Related projects

- [Milo-V2.0](https://github.com/MillenniumMachines/Milo-V2.0) — mechanical mill (electronics not included in that repo)
- [Millennium Machines documentation](https://millenniummachines.github.io/docs/) — published guides (UEB, Milo, and other projects)
- [millenniummachines.github.io](https://github.com/MillenniumMachines/millenniummachines.github.io) — documentation site source

## License

See repository license file when published. Until then, treat CAD and STLs as part of the Millennium Machines open hardware ecosystem and follow project guidance on Discord for use and redistribution.
