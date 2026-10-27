# Fabrication, assembly and verification

## Working with the native FreeCAD design

1. Open `cad/FunnelStrip_Parametric.FCStd` in **FreeCAD** (source drawing reports version **1.0.2**).
2. In the model tree, open the spreadsheet labelled **Dimensions (mm) — edit column B** (object `Parameters`).
3. Main values: `Count`, `Pitch`, `Length`, `Width`, `Thickness`, `Opening`, `ConeOD`, `ShoulderOD`, `Depth`, `SleeveOD`, `Insertion`, `Bore`, `RibThickness`, `RibDepth`, `CornerRadius`.
4. Change one parameter at a time; **recompute**, verify feature status and inspect the section and repeated features.
5. Choose the final body and export as **STEP** for CAD exchange or **STL** for 3D-print preparation. A STEP export is not a substitute for the parameter spreadsheet when changing geometry.

## Manufacturing options

- **Prototype:** 3D print a two-position or full-length test part; dimensional accuracy at the thin sleeves and inlets matters more than cosmetic surface quality.
- **Production/regular sampling:** consider a process and material that provide smooth, chemically compatible, cleanable wetted surfaces. Support removal, layer texture and inaccessible crevices can retain liquid.
- **Fit tuning:** nominal sleeve diameter is 13.8 mm for nominal 14.4 mm tube ID. Allow for build deviation; do not force a sleeve into glass. Check the smallest physical bore, not only the nominal supplier value.
- **Bed size:** a 280 mm-long part may exceed compact printer build volumes; slicing, splitting and joining would change sample carryover/cleanability and must be redesigned and validated.

## Before use

1. Confirm the insert sleeves are dimensionally correct and free of sharp edges.
2. Seat ten glass tubes in the rack; check they do not touch one another.
3. Lower the collector until each locating sleeve enters the tube freely and every shoulder is supported.
4. Check the entire assembled unit for stability and interference.
5. Run water into each inlet independently; check the intended outlet, residue/hold-up and leakage.
6. Move progressively between inlets while collecting; compare carryover and spills under actual operating conditions.

**Safety:** Uncertified 3D-printing polymers and resins are not automatically compatible with drinking liquids, hot liquids, solvents, or sterilization. The native model is not validated for particular temperatures, chemicals, repeated cleaning or metrology. Never force the printed insert into fragile glass.

## Validation results

No formal dimensional inspection or fraction carryover/retention report is included with the initial public design. Community fit reports and tests are welcome via GitHub Issues.
