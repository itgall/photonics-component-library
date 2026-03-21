# Contributing to the Photonics Component Library

Thank you for your interest in contributing. This document provides guidelines for adding new components, reporting issues, and suggesting improvements.

## Adding New Components

New components should follow the established conventions for consistency across the library.

**Naming.** Fiber optics components use the `f-` prefix and free-space components use the `fs-` prefix, followed by a descriptive hyphenated name (e.g., `f-isolator`, `fs-achromatic-doublet`). Names should be lowercase and use hyphens rather than underscores.

**Styles.** Each new component must be provided in all three rendering styles: flat 2D, pseudo-3D (gradient-shaded), and wireframe (black line art). If you are only able to produce one style, please note this in your pull request and another contributor can help complete the set.

**Formats.** Provide SVG as the primary source format. PNG files should be rasterized at 600 pixels wide with transparent backgrounds. Both formats are required for each style.

**SVG standards.** SVG files should be self-contained with no external dependencies. Use standard SVG elements (paths, rectangles, circles, ellipses, polygons) rather than tool-specific extensions. Include a descriptive `<title>` element inside the SVG. Viewbox should be set appropriately with minimal whitespace padding.

**Categorization.** Place new components in the appropriate subcategory folder. If no existing category fits, propose a new one in your pull request description.

## Reporting Issues

If you find an incorrect component, a rendering artifact, a missing variant, or a categorization error, please open an issue with a clear description of the problem and which component(s) are affected.

## Suggesting Improvements

Feature requests, style improvements, and organizational changes are welcome as issues. Please describe the improvement you have in mind and why it would benefit the library.

## Code of Conduct

Please be respectful and constructive in all interactions. This is a community resource built for the benefit of the photonics and optics community.
