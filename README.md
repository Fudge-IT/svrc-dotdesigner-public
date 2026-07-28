# Dot Designer

Dot Designer is a desktop application for creating tactile dot graphics, braille-ready diagrams, and layouts intended for embossing.

It provides a visual dot-based canvas for drawing, editing, tracing, braille entry, and export. The application is designed to make tactile graphics easier to construct while keeping individual dot placement visible and editable.

## Features

### Drawing and Editing

- Pencil and eraser tools with adjustable brush sizes
- Lines, curves, rectangles, ellipses, polygons, stars, hearts, and more
- Configurable solid and patterned fills
- Direct entry of fill density and spacing
- Hollow Shape tool for removing dots from inside existing outlines
- Table generation within the canvas or a selected area
- Unified undo and redo across drawing, braille, and reference-image changes

### Selection and Transformation

- Move selections partially or completely outside the canvas
- Resize selected or pasted dots
- Free rotation with optional 15-degree snapping
- Rotate and flip content extending beyond the canvas
- Cut, copy, paste, and repeated paste workflows
- Preserve unrelated dots beneath moved selections
- Copy raster selections between document tabs

### Multiple Documents

- Work on multiple drawings using tabs in one window
- Rename and reorder tabs
- Reopen recently closed tabs
- Independent undo history, zoom, scroll position, tools, selections, braille, and reference images for each tab
- Copy dots and braille blocks between tabs

### Braille

- Six-key braille entry
- Multiple independently editable braille text blocks
- Move, copy, paste, and reopen braille blocks for editing
- Braille content remains separate from ordinary drawing dots while editing
- Braille is included when exporting the complete canvas or a selected area

### Images

- Place PNG and JPEG reference images for tracing
- Move, resize, rotate, and adjust reference-image opacity
- Add multiple reference images to a project
- Convert images directly into editable dots
- Choose between:
  - **Crisp shapes** for text, logos, diagrams, and clear edges
  - **Shaded detail** for photographs, light, and shadow
- Adjust dot density, inversion, output dimensions, and proportions
- Compare converted dots against a transparent preview of the original image
- Move and resize converted dots before confirming them

### Canvas and Display

- Standard and custom canvas sizes
- Grid and dot-view modes
- Adjustable zoom
- Custom application colours
- Optional safe-width guide for export planning
- Reference images, selections, braille, and drawing dots remain aligned when the canvas is resized

### Import and Export

- Save editable projects as `.dots`
- Open and import supported tactile raster files
- Export the complete canvas as:
  - `.vim`
  - `.brg`
  - `.svg`
- Export selected areas separately
- Optionally trim blank space from selection exports
- Add a configurable dot margin around trimmed exports
- Reference images and visual guides are never included in exports

## Download

Download the latest Windows installer from the [Releases](../../releases) page.

The application currently provides a 64-bit Windows build. macOS builds are not currently distributed through this repository.

## Getting Started

1. Create a new tab or open an existing project.
2. Choose a drawing tool from the toolbar.
3. Draw directly on the dot canvas or import existing content.
4. Add reference images when tracing or positioning a design.
5. Use the braille tool to create editable braille text blocks.
6. Save the editable project as a `.dots` file.
7. Export the complete canvas or a selected region in the required format.

## File Formats

- `.dots` - Editable Dot Designer project containing drawing dots, braille blocks, canvas settings, and reference images
- `.vim` - Fixed tactile raster export format
- `.brg` - Fixed braille/tactile graphics raster format
- `.svg` - Scalable visual export format

Reference images are stored in `.dots` projects but are not included in exported tactile or SVG files.

## Braille and Export Limitations

Braille blocks are independently editable within Dot Designer, but `.vim` and `.brg` are fixed raster formats. Braille and drawing content must therefore be composed onto the dot positions supported by those formats during export.

Physical spacing and final embossed output can also be affected by downstream translation, scaling, embosser configuration, and punch dimensions. Braille spacing should be treated as best-effort within the limitations of the selected export format and production workflow.

Image conversion is intended to provide an editable starting point. Converted graphics may require manual cleanup depending on the source image and desired tactile result.

## Project Status

Dot Designer is feature-complete for its core tactile-graphics workflow. Future updates are expected to focus on usability, compatibility, accessibility, and bug fixes.

This public repository provides release downloads and update metadata. The application source code is maintained privately.
