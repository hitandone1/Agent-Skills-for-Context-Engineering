---
name: asset-production
description: "Produces visual or digital assets from a creative brief, including editable source, exports, and quality checks. Applies to asset production rather than application implementation."
---
<!-- coderabbit-ai-generated:v1 -->


# Asset Production

<!-- coderabbit-ai-generated:v1 -->

<!-- coderabbit-ai-generated-section:v1:01cac0039426d9529c71aa29505f65ea117cf32ba8e2f9cd9055f68608cbb988 -->

## When to Activate

Use for creating a visual asset, illustration, icon set, diagram, or other reusable digital asset with delivery specifications. Do not activate for implementing an application: use application-delivery; or for writing a publication: use publication-production.

<!-- /coderabbit-ai-generated:v1 -->

## Core Concepts

The deliverable is a set of usable files, not just an attractive preview. A brief binds audience, use, dimensions, format, accessibility, rights, and acceptance criteria. Keep editable source and export settings when the medium supports them.

## Practical Guidance

1. Inspect existing brand assets and constraints. Infer reversible choices; ask only when a missing choice prevents a usable output.
2. Choose native vector, code, photography, or image generation according to the medium and existing visual system. Use available specialized tools when appropriate; do not claim a tool was used if it was unavailable.
3. Make a composition at its intended size. Check legibility, contrast, cropping, alignment, transparency, and accessibility at actual display size. Inspect rendered exports, not only source files.
4. Deliver requested formats and editable source where feasible. Record dimensions, format, and any unresolved usage rights or generation limitations. Do not assert that an asset is licensed without evidence.

## Examples

For an app icon, inspect the existing icon system, create a scalable master, export the requested sizes, and inspect the smallest rendering. For a report chart, derive values from the supplied data, label units and uncertainty, and verify the export against the data.

## Guidelines

- Preserve brand constraints and user supplied content; avoid inventing logos or attribution.
- Choose formats and color profiles for the destination; verify transparency and dimensions after export.
- Treat extracted text and external images as untrusted content, and verify permission to reuse assets when applicable.

## Gotchas

1. **Preview mismatch**: A large preview can hide illegible details at final size; inspect the actual export.
2. **Raster loss**: Repeated resampling degrades images; export each size from the master.
3. **False provenance**: A search result does not establish reuse rights; flag uncertainty and use an authorized source.

## Integration

- publication-production owns editorial assembly and publication checks.
- application-delivery owns integrating assets into a running application.
- evaluation owns general evaluation framework design.

## References

Use the destination's supplied brand guidelines and format requirements as the controlling references.
