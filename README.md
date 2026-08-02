# CalSol Aux Battery Pack Notes

## Scope

This folder appears to be a working set for the auxiliary battery pack used on CalSol Berkeley's vehicle.

Project context provided with this folder:

- Made right before FSGP 2026
- Iterated during FSGP 2026
- Battery inside the pack is lead-acid

The notes below only include information that is either:

- directly visible in the files in this folder, or
- provided in the project context above

## What Is In This Folder

### Aux pack CAD iterations

- `aux assembly - 1.zip`
- `aux assembly - 2.zip`

Each ZIP contains the same 4 SolidWorks files:

- `aux assembly.SLDASM`
- `aux enclosure bottom.SLDPRT`
- `aux enclosure top.SLDPRT`
- `aux.SLDPRT`

### Other related CAD/reference files

- `ASM.SLDASM`
- `ASM - Small.SLDASM`
- `Box V3.SLDPRT`
- `Box V3 - Small.SLDPRT`
- `EXP12200 Mockup.SLDPRT`
- `Miady 12V 7Ah Rechargeable Sealed Lead Acid Battery.SLDPRT`
- `EXP12200.pdf`
- `Miady 12V 7Ah Rechargeable Sealed Lead Acid Battery Size.jpg`
- `Reg.png`

## Confirmed Battery Information

### Battery chemistry

- The battery is lead-acid according to project context.
- The image file `Miady 12V 7Ah Rechargeable Sealed Lead Acid Battery Size.jpg` shows a sealed lead-acid battery.

### Battery details visible in the Miady reference image

From `Miady 12V 7Ah Rechargeable Sealed Lead Acid Battery Size.jpg`:

- Battery type shown: sealed lead-acid battery
- Visible model text: `SLA12V7AH`
- Nominal rating shown: `12V 7Ah`
- Terminal type shown: `F2`
- Weight shown: `4.19 lbs`
- Dimensions shown:
  - Length: `5.94 in` (`15 cm`)
  - Width: `2.55 in` (`6.5 cm`)
  - Height: `3.74 in` (`9.5 cm`)

### Other battery references present

- `EXP12200.pdf` is present and appears to be a battery reference/spec sheet.
- `EXP12200 Mockup.SLDPRT` is present and appears to be a CAD mockup for that battery reference.

The file names strongly suggest `EXP12200` was another battery reference used during packaging work, but the full PDF text could not be cleanly extracted in this environment, so detailed specs from that file are not listed here.

## Enclosure / Rules Reference

`Reg.png` is a screenshot of `ASC 2026` rules section `8.4 Battery Enclosures` and `8.5 Cooling`.

The visible requirements in that screenshot include:

- Registered and sealed battery modules, supplemental batteries, battery protection circuitry, and main fuses must be fully contained in electrically isolated enclosures.
- The inside of the enclosure must be non-conductive.
- No more than two separate enclosures are allowed for the main and supplemental batteries.
- Resistance between battery terminals and chassis must be greater than `100 ohms per 1 volt` of maximal battery potential.
- Enclosures must be secured to the chassis and designed so they do not come loose in an accident or rollover.
- Mounting should consider a `5G` impact in the forward or vertical direction.
- Nylon luggage-type buckles are not accepted for securing the enclosure.
- The top of each battery enclosure must be marked with hazard text including `Caution: Chemical Hazard` and `High Voltage`, plus battery type.
- Main battery enclosure ventilation requirements are shown in the screenshot.
- A seal is required to indicate unauthorized access/contravention.

This screenshot is useful as a design/compliance reference for the enclosure, even though it says `ASC 2026` rather than `FSGP 2026`.

## Revision Trail Visible From The ZIP Files

### `aux assembly - 2.zip`

Contained file timestamps:

- `aux.SLDPRT`: `2026-06-24 08:28`
- `aux enclosure bottom.SLDPRT`: `2026-06-24 09:12`
- `aux assembly.SLDASM`: `2026-07-08 20:00`
- `aux enclosure top.SLDPRT`: `2026-07-08 20:00`

This looks like an iteration where some core part files started in late June 2026, then the assembly and top enclosure were updated on July 8, 2026.

### `aux assembly - 1.zip`

Contained file timestamps:

- `aux enclosure bottom.SLDPRT`: `2026-07-09 01:41`
- `aux.SLDPRT`: `2026-07-09 01:41`
- `aux enclosure top.SLDPRT`: `2026-07-09 01:43`
- `aux assembly.SLDASM`: `2026-07-09 01:45`

This is the later archived iteration in this folder. All four aux-pack files were updated on July 9, 2026.

### Practical takeaway

- `aux assembly - 2.zip` appears to be the earlier archived state.
- `aux assembly - 1.zip` appears to be the later archived state.
- The aux pack design was actively revised across late June to early July 2026.

## Likely Structure Of The Design Set

Based on filenames, the aux battery pack design likely includes:

- A battery or battery placeholder part: `aux.SLDPRT`
- A two-piece enclosure:
  - `aux enclosure bottom.SLDPRT`
  - `aux enclosure top.SLDPRT`
- A full assembly:
  - `aux assembly.SLDASM`

Other top-level files such as `Box V3`, `Box V3 - Small`, `ASM`, and `ASM - Small` look like separate enclosure/packaging studies or variant assemblies.

## What Was Not Found

- No obvious video files were present in this folder.
- No text notes or documents explicitly naming `CalSol`, `Berkeley`, or `FSGP 2026` were found in the files themselves.
- No extracted BOM, drawing, or manufacturing notes were found.

## Short Summary

This folder contains a small aux battery pack design set centered around a lead-acid battery enclosure and assembly. The clearest battery reference visible here is a sealed lead-acid `12V 7Ah` Miady battery with `F2` terminals and dimensions `5.94 x 2.55 x 3.74 in`. The archived SolidWorks files show at least two aux-pack iterations across late June and early July 2026, with the later archive dated July 9, 2026. A rule screenshot for `ASC 2026` battery enclosure requirements is also included and likely informed the enclosure design.
