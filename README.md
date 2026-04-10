# Photonics Component Library

An open-source vector graphics library of **photonics and optics components** for scientific diagrams, technical illustrations, and publication-quality figures. Every component is provided in three rendering styles (flat 2D, pseudo-3D, and wireframe) and two formats (SVG and PNG).

## Overview

| | Components | Styles | Formats | Total Files |
|---|---|---|---|---|
| **Unified Library** | 879 | 3 | 2 | 5,274 |
| **Fiber Optics** | 489 | 3 | 2 | 2,934 |
| **Free-Space Optics** | 390 | 3 | 2 | 2,340 |

The library attempts to cover virtually every component encountered in modern photonics laboratories and systems, organized into clearly labeled categories for easy browsing.

## Rendering Styles

Each component is available in three styles optimized for different use cases.

**Flat 2D** provides clean, filled shapes with distinct colors for each functional element. Best suited for system-level schematics and presentation slides where clarity and readability are priorities.

**Pseudo-3D** uses gradient shading to suggest depth and volume. This style works well for technical reports and journal publications where a polished, professional appearance is desired.

**Wireframe** renders components as black line art on a white background, following the conventions of journal-quality technical drawings. This style is ideal for manuscripts, patent filings, and any context where minimal ink usage or black-and-white reproduction is required.

## Library Organization

### Fiber Optics (`fiber-optics/`)

489 components covering the full scope of fiber-based photonics, organized into 41 subcategories under 12 top-level groups.

| Category | Components | Description |
|---|---|---|
| 01 — Fiber Types | 106 | Standard, specialty, gain, mid-IR, doped, and application-specific fibers |
| 02 — Connectors | 28 | Single-fiber (FC, SC, LC), multi-fiber (MPO), high-power, and adapters |
| 03 — Passive Components | 58 | Couplers, isolators, circulators, WDM, filters, attenuators, switches, polarization |
| 04 — Active Components | 45 | Modulators (EOM, AOM, MZM), amplifiers (EDFA, YDFA, Raman), pump sources |
| 05 — Laser Sources | 43 | DFB, DBR, VCSEL, ECL, fiber laser cavities, saturable absorbers |
| 06 — Detectors & Receivers | 15 | Photodetectors, APD, balanced receivers, coherent DSP |
| 07 — Transceivers & Networking | 39 | SFP through CFP8 modules, ROADM, WSS, OLT/ONU |
| 08 — Packaging | 6 | Butterfly, TO-can, hermetic housings |
| 09 — Gratings & Sensors | 31 | FBG variants, physical sensors, distributed sensing (DTS, DAS, BOTDA) |
| 10 — Test & Measurement | 50 | OSA, OTDR, oscilloscopes, RF analyzers, characterization instruments |
| 11 — Infrastructure | 53 | Splicing, cable management, inline components, beam delivery, thermal |
| 12 — Quantum & Specialty | 15 | Quantum sources, QKD, specialty fiber systems |

### Free-Space Optics (`free-space-optics/`)

390 components covering the full scope of bulk and free-space optics, organized into 71 subcategories under 20 top-level groups.

| Category | Components | Description |
|---|---|---|
| 13 — Lenses | 23 | Singlet, aspheric, achromatic, cylindrical, objectives, imaging |
| 14 — Mirrors | 20 | Flat, curved, OAP, scanning, flip, adaptive (DM) |
| 15 — Beamsplitters | 7 | Non-polarizing (plate, cube, pellicle), polarizing (PBS) |
| 16 — Prisms | 18 | Steering, dispersive, polarizing (Wollaston, Glan-Taylor, etc.) |
| 17 — Polarization | 17 | Waveplates, compensators, polarizers, isolators, depolarizers |
| 18 — Filters | 14 | Interference, ND, absorptive, tunable (LCTF, AOTF) |
| 19 — Gratings | 6 | Blazed, transmission, echelle, VPH, concave, grism |
| 20 — NLO Crystals | 34 | SHG/SFG, OPO/DFG, Raman crystals, accessories |
| 21 — EO/AO Devices | 11 | Pockels cells, AOMs, pulse pickers, cavity dumpers |
| 22 — SLM & Beam Shaping | 16 | LCoS, DMD, DOE, microlens arrays, diffusers |
| 23 — Apertures & Beam Control | 8 | Iris, spatial filter, beam dump, chopper, stabilizer |
| 24 — Windows | 19 | CaF₂, ZnSe, Ge, Si, sapphire, diamond, BaF₂, and more |
| 25 — Detectors & Cameras | 37 | Photodiodes, thermal, IR, single-photon, cameras, wavefront sensors |
| 26 — Laser Sources | 44 | Gas, solid-state, semiconductor, tunable/broadband, THz |
| 27 — Optomechanical | 24 | Mounts, stages, posts, cage systems, breadboards |
| 28 — Beam Delivery | 17 | Expanders, scanners, alignment tools, transport |
| 29 — Interferometric | 15 | Etalons, delay stages, Michelson, Mach-Zehnder, Sagnac, etc. |
| 30 — Spectroscopy | 24 | Light sources, monochromators, spectrometers, sample cells |
| 31 — Quantum Optics | 15 | SPDC sources, Bell analyzers, HBT correlators, QKD |
| 32 — Adaptive/Astro/Industrial | 21 | Deformable mirrors, coronagraphs, cutting heads, safety |

### Unified Library (`unified/`)

All 879 components in a single organized tree with both `fiber/` and `freespace/` subdirectories. Use this when you want access to the complete collection in one location.

## Naming Convention

Fiber optics components use the `f-` prefix (e.g., `f-dfb-laser.svg`, `f-isolator.svg`). Free-space optics components use the `fs-` prefix (e.g., `fs-flat-mirror.svg`, `fs-achromatic-doublet.svg`). This ensures zero name collisions when both libraries are used together.

## Directory Structure

```
photonics-component-library/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── unified/
│   ├── flat_2d/
│   │   ├── svg/
│   │   │   ├── fiber/
│   │   │   │   ├── 01_standard_fibers/
│   │   │   │   ├── 01_specialty_fibers/
│   │   │   │   └── ...
│   │   │   └── freespace/
│   │   │       ├── 13_singlet_lenses/
│   │   │       ├── 14_flat_mirrors/
│   │   │       └── ...
│   │   └── png/
│   │       └── (same structure as svg/)
│   ├── pseudo_3d/
│   │   └── (same structure as flat_2d/)
│   └── wireframe/
│       └── (same structure as flat_2d/)
├── fiber-optics/
│   ├── flat_2d/
│   │   ├── svg/
│   │   │   ├── 01_standard_fibers/
│   │   │   └── ...
│   │   └── png/
│   ├── pseudo_3d/
│   └── wireframe/
└── free-space-optics/
    ├── flat_2d/
    │   ├── svg/
    │   │   ├── 13_singlet_lenses/
    │   │   └── ...
    │   └── png/
    ├── pseudo_3d/
    └── wireframe/
```

## Usage

All SVG files are self-contained vector graphics that can be opened in any SVG-compatible editor or viewer, including Adobe Illustrator, Inkscape, Affinity Designer, and web browsers. PNG files are rasterized at 600 pixels wide with transparent backgrounds.

To use a component in your diagram, simply copy the SVG file into your illustration project, or drag the PNG into a presentation or document.

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt the material for any purpose, including commercial use, provided you give appropriate credit.

## Contributing

Contributions are welcome. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding new components, reporting issues, or suggesting improvements.

## Citation

If you use this library in a publication, we appreciate (but do not require) a citation or acknowledgment. A suggested format:

> Photonics Component Library (2025). Available at: https://github.com/itgall/photonics-component-library
