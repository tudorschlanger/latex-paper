# LaTeX template for academic papers

This repository contains a minimalist template to write academic papers with LaTeX. 

The template was initially forked from Pascal Michaillat (see license), but it has been adapted to incorporate my personal preferences. 

## Main files and how to use them

- `paper.tex` –  Skeleton of the paper. Fill it out the title page and abstract. Use the subfiles to fill in the rest of the paper. 
- `paper.sty` –  LaTeX style file collecting all the formatting commands. Must be included in the same folder as `paper.tex`.
- `1_intro.tex`, `2_data.tex`, `3_model.tex`, `4_empirics.tex`, `5_conclusion.tex`, `6_appendix.tex` are the subfiles which map the main skeleton of the paper; these are called in `paper.tex` and can be added or removed as needed.  

## Additional files for online appendix

Bibliography files: 
- `bibliography.bib` – BibTeX file with all the references included in the paper. Replace the references with your own.
- `bibliography.bst` – BibTeX style file to format the entries into the reference section. This style file is [hosted in this GitHub repository](https://github.com/pmichaillat/latex-bibliography). 

The repository also includes an additional template and style file in case the appendix of the paper must be carved out into a separate online appendix. 

- `online_appendix.tex` –  Skeleton of the online appendix. Fill it out with the content of your online appendix. The appendix must be in the same folder as the paper so the equation and section labels from the paper can be used in the online appendix.
- `appendix.sty` –  LaTeX style file collecting additional formatting commands for the online appendix. Must be included in the same folder as `appendix.tex`. This style file must be used in conjonction with `paper.sty`, which must also be included in the folder. 

## Key features

- The font for text, roman math, and numbers is [Source Serif Pro](https://fonts.google.com/specimen/Source+Serif+Pro).
- The font for Greek and calligraphic math is [Euler](http://luc.devroye.org/fonts-26139.html).
- No colors are used in the text (only black) to reduce distraction, and so papers print well.
- Colors are reserved for graphs.
- Margins, spacing, and font size are set for comfortable reading.
- Formatting is also specified for appendix and online appendix.

## Reference

As much as possible the style file follows Matthew Butterick's wonderful typographical advice in [Practical Typography](https://practicaltypography.com).
