# EPFL - Unofficial Report/Thesis Template (v1.1.0)

This template aims to adapt TU Delft Report Template to EPFL. Some of the main features:

* **Simplicity First:** A class file that has been reduced by nearly 70% to simplify customization;
* **Effortless:** A careful selection of common packages to get started immediately;
* **Complete:** Ready-to-go when it comes to the document and file structure.

This template works with _pdfLaTeX_, _XeLaTeX_ and _LuaLaTeX_. In order to adhere to the TU Delft house style, either _XeLaTeX_ or _LuaLaTeX_ is required, as it supports TrueType and OpenType fonts. _BibLaTeX_ is used for the bibliography with as backend _biber_. Please visit https://dzwaneveld.github.io/report/ for the full documentation.

## Documentation (Abridged)

*→ Visit https://dzwaneveld.github.io/report/ for the full documentation.*

As a report/thesis is generally a substantial document, the chapters and appendices have been separated into different files and folders for convenience. The folders are based on the three parts in the document: the frontmatter, mainmatter and appendix. All files are inserted in the main file, `report.tex`, using the `\input{filename}` command. The document class, which can be found in `tudelft-report.cls`, is based on the `book` class.

The template will automatically generate a cover when the `\makecover` command is used. The title, subtitle and author will also be present on the title page. To give greater flexibility over the title page, the layout is specified in `title-report.tex`. A title page for theses is also available: `title-thesis.tex`. Change the corresponding `\input{...}` command in the main file to switch. 

The bibliography has been set up in `report.tex` to allow for easy customization. It is included in the table of contents and renamed to 'References' using the `heading=bibintoc` and `title=References` options of the `\printbibliography` command respectively. If you would like to use a different `.bib` file, change the command `\addbibresource{report.bib}` accordingly. 

## License

This work is based of Daan Zwaneveld's [TU Delft - Unofficial Report/Thesis Template](https://github.com/dzwaneveld/TU-Delft-Unofficial-Report-Template)

This repository will stay a fork of the original repository in order to pull updates to the original template.

This template is available under CC BY-NC 4.0. For more information, see https://creativecommons.org/licenses/by-nc/4.0/. No attribution is required in reports/theses created using this template.
