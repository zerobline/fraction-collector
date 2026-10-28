# Repository settings and release checklist

## Current publication status

The following files are published in the public repository on `main`:

- [Native FreeCAD model](../cad/FunnelStrip_Parametric.FCStd)
- [Original PDF drawing](../cad/FunnelStrip_Drawing.pdf)
- [STEP export](../cad/FunnelStrip_Final.step)
- [STL export](../cad/FunnelStrip_Final.stl)
- [PNG](FunnelStrip_Drawing.png) and [SVG](FunnelStrip_Drawing.svg) drawing previews

The source, original PDF and exports have been uploaded; **no additional CAD upload is required** for repository browsing or downloads.

## Suggested GitHub metadata

- **Description:** Open-source FreeCAD 10-position test-tube funnel strip for sequential liquid fraction collection; compatible rack and tube part references.
- **Website:** optional; leave blank unless hosted documentation is available.
- **Topics:** `freecad`, `cad`, `open-hardware`, `fraction-collector`, `test-tubes`, `3d-printing`, `lab-equipment`, `parametric-design`, `sample-collection`.
- **Visibility:** Public.
- **Default branch:** `main`.
- **Features:** Issues enabled; Wiki/Discussions optional.
- **License:** MIT (see [LICENSE](../LICENSE)); external supplier names and materials remain third-party content.

Repository description and topics may still need setting using **Repository → About → gear**. The connected GitHub file editor cannot change repository metadata.

## Future versioned release

A first numbered release is optional: visitors can already download the files from the `main` branch. Before publishing a `v1.0.0` release, check the following:

- [x] Native FreeCAD source and PDF uploaded
- [x] STEP and STL exports uploaded
- [x] PNG and SVG preview drawings uploaded
- [ ] Open/recompute native file on the intended FreeCAD version
- [ ] Verify measured pitch (nominal 27 mm) and tube-mouth sleeve clearance
- [ ] Pass physical two-position fit check, then full ten-position check
- [ ] Check flow through all ten passages and quantify retained liquid/carryover
- [ ] State material, manufacturing process and fluid/temperature limitations
- [ ] Export the release STEP/STL from the verified native model

Use [Issues](https://github.com/zerobline/fraction-collector/issues) to report fit measurements or document a reproducible test. Keep the model and engineering drawing revision synchronized if geometry changes.
