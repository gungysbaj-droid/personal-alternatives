# Candidate gaps, not a cloning backlog

Research snapshot: 2026-10-13. These are small build opportunities, not claims that no alternatives exist. No hands-on benchmarking was done. Validate a real unmet need before writing an app.

| Candidate | What already exists | Opportunity to validate | First useful slice |
| --- | --- | --- | --- |
| Motion-design workflow | Natron already offers node-based compositing, tracking, roto, keying, keyframes and OFX plugins. An independent review finds that text animators, shape layers and expression-driven motion do not map to its workflow like they do in After Effects. | A small, friendly typography/keyframe workflow rather than a new compositor. This is the best candidate if reusable animated titles are a real need. | Animate one text block with per-character delay, easing and deterministic frame export. Save the project as documented JSON. |
| Local PDF workflow | PDF Arranger already handles merge/split/crop/rotate/reorder. Stirling PDF lists text editing, OCR, redaction, forms and certificate signing, although tool availability depends on deployment. | Do not assume "PDF editing is missing". Test one end-to-end local workflow for friction, privacy and output fidelity; build only the missing piece. | A batch organizer with an explicit operation plan and export checks. Redaction/signature correctness is a separate, higher-risk project, not a casual first feature. |
| Portable design handoff | Inkscape already has multipage design and PDF export. Its multipage SVG representation uses Inkscape-specific metadata; browsers display only the first page. | A standards-oriented export/manifest helper for sharing multipage assets without relying on one editor's project format. | Export separate page SVGs plus a manifest and contact sheet; verify fonts, page bounds and ordering on a test fixture. |

## Recommendation

Keep the scaffold and choose nothing yet if existing tools meet the need. When a pain point appears, test existing software on a small fixture first. Prefer a plugin, wrapper or focused component over a full Photoshop/After Effects/Acrobat replacement. REA is optional and useful only when an authorized behavior investigation answers a specific question.

## Sources and limits

- [Natron official site](https://natrongithub.github.io/): the existing 2D compositing/keyframe/OFX feature set. This is not evidence that every motion-design task is missing.
- [XDA, February 8, 2026](https://www.xda-developers.com/adobe-after-effects-alternative-create-motion-graphics-for-free/): one user's workflow comparison, including text/shape/expression and 3D tradeoffs. Experience report, not a controlled benchmark.
- [PDF Arranger](https://github.com/pdfarranger/pdfarranger): page-organization scope; GPL-3.0 metadata. Linking is not permission to copy its code into an MIT project.
- [Stirling PDF tool catalog](https://docs.stirlingpdf.com/Tools/): broad PDF coverage and deployment-dependent availability. It would be wrong to label PDF editing or OCR categorically absent.
- [Stirling PDF license](https://github.com/Stirling-Tools/Stirling-PDF/blob/main/LICENSE): multiple directory-specific licenses; do not assume the entire codebase is MIT.
- [Inkscape multipage documentation](https://wiki.inkscape.org/wiki/Multipage): multipage editing/export and browser portability caveat. Verify against the installed version before implementation.

These are candidate opportunities inferred from documented workflows. They are not proven market gaps, legal advice, or a commitment to build. No urgency to beat a vendor patch has been established.
