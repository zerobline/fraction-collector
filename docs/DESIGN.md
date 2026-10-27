# Design specification and provenance

This is the **final user-created FreeCAD revision**, not an earlier generated concept or AI illustration. The authoritative native document is `FunnelStrip_Parametric.FCStd`, which includes a FreeCAD **Parameters** spreadsheet, Part Design features, repeated patterns, and a TechDraw page. Drawing reference **FS-001 | Rev B | 2026-10-27**.

## Key dimensions

| Feature | Value | Source/status |
|---|---:|---|
| Stations | 10 | Final CAD |
| Pitch | 27 mm | Final CAD; rack measurement **approximate** |
| Strip length | 280 mm | Final CAD |
| Strip width | 29 mm | Final CAD |
| Strip thickness | 3 mm | Final CAD |
| Top opening diameter | 27 mm | Final CAD (opening equals pitch) |
| Outer cone top diameter | 29 mm | Final CAD |
| Shoulder diameter | 17 mm | Final CAD |
| Depth below strip to shoulder | 9 mm | Final CAD |
| Sleeve outside diameter | 13.8 mm | Final CAD; physical fit not yet validated |
| Sleeve insertion depth | 6 mm | Final CAD |
| Drain bore diameter | 10 mm | Final CAD |
| Inner throat offset | 1 mm | Final CAD |
| Connecting rib thickness | 3 mm | Final CAD |
| Connecting rib depth | 7.2 mm | Final CAD |
| Overall model height | 18 mm | Final CAD (3 + 9 + 6) |
| End corner radius | 5 mm | Final CAD |
| Rack overall L × D × H | 280 × 70 × 84 mm | Tuuters E51016 supplier table |
| Rack hole diameter | 16.5 mm | Tuuters E51016 supplier |
| Rack pitch | ~27 mm | Estimated from ruler photographs; not confirmed engineering tolerance |
| Tube length × OD × nominal ID | 120 × 16 × 14.4 mm | Tuuters smooth-rim size table |

The spreadsheet contains some **legacy unused tab parameters**. Edit only parameters used by the feature tree and check recompute status before exporting.

## Geometric principle

An upper plate joins **10 round, adjacent, nominally tangent inlets**. Each station has its own conical underside and through passage, finished with a cylindrical sleeve and shoulder. The intent is for a small moving stream to be intercepted while the row is advanced incrementally, without ten separately mounted funnels.

The nominal **Ø17 mm shoulder** rests at/over the outside of the **Ø16 mm** tube rim, while the **Ø13.8 mm sleeve** locates inside the nominal **Ø14.4 mm** tube bore. Nominal radial clearance: **0.30 mm**. This is not a tolerance fit: no measured minimum bore, tube lip runout, printed diameter error or distortion allowance is available.

On 10 equally spaced centers, first-to-last centers span **9 × 27 = 243 mm**; assuming symmetry on a 280 mm rack would leave **18.5 mm** from each outside edge to the nearest center. This end offset is a *calculated assumption*, not an independently measured value.

## Requirements before manufacture

1. Measure rack first/last center distance and check the intermediate centers; do not infer fit solely from rack length.
2. Verify tube **minimum** internal diameter and lip shape with the actual product and the manufacturing process's tolerances.
3. Check the assembled height against liquid inlet clearance.
4. Print or machine a two-position fit-check coupon before the full ten-position part.
5. Confirm **each passage is open** after manufacture and clean the part thoroughly.
6. Quantify carryover across stations, retained liquid, splash and drain-down time using a harmless test fluid.
7. Select material for temperature, liquid compatibility and cleaning (not all printed plastics or resins qualify).

## Known limitations

The inlet rims touch and can support liquid bridges or residual films between samples; **independent bore geometry does not guarantee zero sample carryover**. The model is a passive collector with no timed/indexing mechanism, seals, flow measurement or proof of analytical accuracy.

The drawing is a general arrangement, not a complete manufacturing tolerance and acceptance specification. For authoritative geometry and editable dimensions use the native CAD project.

## Traceability

- FreeCAD drawing: FS-001, revision B, dated 2026-10-27.
- Supplier rack: https://www.tuuters.de/reagenzglashalter/aus-acryl/acrylhalter-ohne/10-loch-acryl-reagenzglashalter-16-in-einer-reihe.html
- Supplier tubes: https://www.tuuters.de/reagenzglaeser/reagenzglaeser-ohne.html
