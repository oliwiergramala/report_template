# LaTeX University Report Template

This repository is a LaTeX template created for writing university reports at the University of Technology in Koszalin.
However, it can be easily adapted for use at any university.

The template is structured in a modular way to separate content, layout, and configuration, making it easy to reuse and maintain.

## Repository Structure

The repository contains the following files and directories:

- main.tex – main document file
- header.tex – title page template
- packages.tex – LaTeX packages configuration
- images/ – directory for images

## File Descriptions

### main.tex

This is the main document file.
All other files are imported here.

It contains:
- Document configuration
- Variable definitions (e.g. title, author, etc.)
- Section content
- Imports of header.tex and packages.tex

This is the only file you typically modify when writing a report.

### header.tex

This file defines the title page.
Its content depends on variables defined in main.tex, such as:

- `\thetitle`
- `\theauthor`
- `\thedate`

The key advantage of this approach is reusability.

You can:
- Import header.tex into multiple main files (e.g. main.tex, main2.tex)
- Change only the variable values in each main file
- Keep the header layout unchanged

There is no need to modify header.tex when creating a new report — only update the variables in the main document.

### packages.tex

This file contains all required LaTeX packages for building the project.

### images/ Directory

All images used in the document should be placed inside the images/ directory.

## Custom Image Macro

A simple macro was created to make inserting images easier:

Example:

```LaTeX
    \image{logo.png}{University logo}
```

This will:
- Insert images/logo.png
- Center the image
- Add an automatically numbered caption
- Keep consistent formatting throughout the document

## How to Use

1. Clone the repository
2. Open main.tex
3. Update the variables (title, author, etc.)
4. Write your report content
5. Compile using your preferred LaTeX compiler (e.g. pdflatex)

The modular design ensures minimal changes are required.
