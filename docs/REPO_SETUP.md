# GitHub repository settings and publishing checklist

## Suggested repository metadata

- **Description:** Open-source FreeCAD 10-position test-tube funnel strip for sequential liquid fraction collection; compatible rack and tube part references.
- **Website:** leave blank until you create a public build guide or hosted documentation.
- **Topics:** `freecad`, `cad`, `open-hardware`, `fraction-collector`, `test-tubes`, `3d-printing`, `lab-equipment`, `parametric-design`, `sample-collection`.
- **Visibility:** Public.
- **Default branch:** `main`.
- **Features:** Issues enabled; Wiki optional; Discussions optional.
- **Licensing:** MIT for the project author's original files; supplier trademarks and externally linked pages remain third-party material.

GitHub app permissions used to add source documentation **do not expose repository settings mutations**. To set description/topics go to **Repository → About → gear**. For Issues go to **Settings → General → Features**.

## Publishing the supplied source assets

The connected GitHub content writer supports UTF-8 text edits, but the native **.FCStd** and **.pdf** attachments require a binary file upload by the maintainer.

1. Open [the repository](https://github.com/zerobline/fraction-collector).
2. Use **Add file → Upload files** and place the two original files at:
   - `cad/FunnelStrip_Parametric.FCStd`
   - `cad/FunnelStrip_Drawing.pdf`
3. Optional preview: `docs/FunnelStrip_Drawing.png` (from the original drawing).
4. Commit to `main`; verify README links resolve.
5. If distributing a release, create a **v1.0.0** GitHub Release after fit-checking, attach STEP/STL exports and a ZIP of native file and drawing, and document tested material/process.

Until step 2 is complete, **CAD file links in the README intentionally point to reserved file paths** and are not downloadable from GitHub.

## First release acceptance checklist

- [ ] Native FreeCAD source present and opens/recomputes
- [ ] Engineering drawing matches native document
- [ ] 27 mm rack pitch verified physically (or tolerance note retained)
- [ ] Sleeve measured in the actual glass tubes
- [ ] Two-position fit check passed
- [ ] All ten passages open
- [ ] Material and fluid compatibility stated
- [ ] Released binaries derived from the native model, not an independently generated illustration
