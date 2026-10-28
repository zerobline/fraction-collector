# CAD files — original model and exports

The four original/released design files are available in this folder.

| File | Description |
|---|---|
| [`FunnelStrip_Parametric.FCStd`](FunnelStrip_Parametric.FCStd) | **Authoritative editable model.** Native FreeCAD document with a `Parameters` spreadsheet and TechDraw sheet. |
| [`FunnelStrip_Drawing.pdf`](FunnelStrip_Drawing.pdf) | Original A3 engineering drawing, **FS-001, Rev B, 2026-10-27**. |
| [`FunnelStrip_Final.step`](FunnelStrip_Final.step) | Solid geometry exported from the finalized FreeCAD document, for interchange with other CAD applications. |
| [`FunnelStrip_Final.stl`](FunnelStrip_Final.stl) | Triangle mesh exported from the finalized model, for 3D printing. This format is not parametrically editable. |

A [PNG preview](../docs/FunnelStrip_Drawing.png) and [SVG drawing](../docs/FunnelStrip_Drawing.svg) are available under `docs/`.

## Editing

Open the `.FCStd` file in FreeCAD (the source drawing reports **FreeCAD 1.0.2**). Edit the `Parameters` spreadsheet, recompute the document and check the final solid and TechDraw views before exporting new STEP/STL files. See [fabrication and validation](../docs/FABRICATION.md).

**Do not confuse the initial prototype concepts with this final user-edited model.** The native FreeCAD file is the source of truth; exports can be regenerated when dimensions change.

The **27 mm rack pitch** was estimated from physical ruler photographs rather than a manufacturer tolerance drawing. Tube-mouth fit and liquid carryover still require physical validation. See [design notes](../docs/DESIGN.md).
