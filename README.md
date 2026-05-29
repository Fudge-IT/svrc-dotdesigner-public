# Dot Designer

Dot Designer is a desktop app for creating tactile dot graphics and braille-ready diagrams.

It is designed for workflows where dot placement matters, with tools for drawing, editing, tracing from reference images, adding braille text, and exporting diagrams for tactile production.

## Features

- Dot-based canvas for tactile graphics
- Drawing tools for lines, curves, shapes, fill, selection, and more
- Braille text blocks with six-key entry
- Reference images for tracing and layout guidance
- Export to `.vim`, `.brg`, and `.svg`
- Export selection with optional blank-space trimming and margins
- Custom canvas sizes and visual guide options

## Download

Download the latest version from the [Releases](../../releases) page.

Windows builds are currently provided. macOS builds may be added in a future release.

## Basic Usage

1. Create or open a Dot Designer project.
2. Draw using the toolbar tools.
3. Add reference images if needed for tracing or layout.
4. Use the braille tool to place editable braille text blocks.
5. Save your project as a `.dots` file.
6. Export the full canvas or a selected region.

## File Formats

- `.dots` - Dot Designer project file
- `.vim` - tactile graphics export format
- `.brg` - braille/tactile graphics export format
- `.svg` - scalable visual export format

## Braille and Export Notes

Braille text in Dot Designer is handled as a separate editable overlay so it can be moved and edited independently from drawing dots.

When exporting to fixed raster formats such as `.vim` or `.brg`, braille placement is converted into the available dot/cell grid. Because these formats and downstream embossing workflows have fixed spacing constraints, physical output may vary slightly. Braille spacing should be considered best-effort within those export limitations.

Reference images are for tracing and layout only. They are not included in exported files.

## Project Status

Dot Designer is feature-complete for its initial workflow. Future updates are expected to focus on bug fixes, polish, and compatibility improvements.
