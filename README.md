# BIBEMME #
## Biblatex styles for journals of environmental microbiology and microbial ecology ##

Biblatex is the modern way of working with citations in LaTeX documents. Together with biber it completely replaces the old BibTeX facilities. While it is easy to use and almost unlimited in flexibility it offers a relatively restricted number of citation styles. Unlike simply using biblatex, writing new citation styles is time consuming and non-trivial to the novice user. The aim of this project is to develop comprehensive citation styles to leading journals of environmental microbiology and microbial ecology requiring little to no tweaking on the user's side.

All styles are designed to work with [biblatex](http://bit.ly/Sn6Bjx) 2.3 and above together with [biber](http://bit.ly/SjJLe6).  
In constructing the styles I referred to the author guidelines of each journal but also to publications from latest issues, as there are occasional conflicts or missing guidelines regarding some types of sources or special cases. Each style defines explicitly the formatting of only the following bibtex reference types: article, book, incollection and inproceedings. Other types are too rare, and in any case are usually not formally described in the author guidelines.


** Disclaimer **
This project as a whole and each style in particular are under continuous development and might therefore contain mistakes or bugs. Please report if you find any bug or missing feature.

Copyright (C) 2012 Roey Angel  
angel[AT]mpi-marburg.mpg.de

THIS PROGRAM COMES AS IS WITH ABSOLUTELY NO WARRANTY.
This software is distributed under the terms of the [The LaTeX Project Public License].

This project was inspired by Timothée Poisot's [ecobiblatex] and I used his geb.bbx as a template.

### Usage: ###
Please refer to .bbx file of each individual style for specific usage instructions.  

1. Place the .bbx and .cbx files in your tex path (e.g. `$TEXMFLOCAL/tex/latex/biblatex` in linux) and add the following to the preamble:  
`\usepackage[style=STYLE_NAME, natbib=true, backend=biber]{biblatex}`  
`\addbibresource{YOUR_BIB_FILE.bib}`
The style and .bib source names should, of course, be replaced by the desired citation style and your personal bibtex collection file.  
2. For styles requiring journal name abbreviations (all styles at the moment), the appropriate `JourAbs-AB_STYLE.map` file or a link to it must be placed withing the same directory as the LaTeX document, where 'AB_STYLE' refers to the specific abbreviation style used by the journal.  
3. Add a bibliography list in the document using: `\printbibliography[sorting=SORT_SCHEME]`. Typically the references should be sorted using `\printbibliography[sorting=nyt]` but note that some styles might require a different sorting scheme (e.g. emi).

## Currently available styles ##

1. emi:     [*Environmental Microbiology*]
2. ismej:   [*The ISME Journal - Multidisciplinary Journal of Microbial Ecology*]
3. femsme:  [*FEMS Microbiology Ecology*]
4. aem:     [*Applied and Environmental Microbiology*] - *NEW! Conforms to the new 2013 citation scheme*
5. tufte-handout: [*Tufte handouts style*] - not a journal but I use this document class for my own notes.

[biblatex]: http://bit.ly/Sn6Bjx
[biber]: http://bit.ly/SjJLe6
[The LaTeX Project Public License]: http://bit.ly/U8CgHn
[ecobiblatex]: http://bit.ly/10TlcHw
[*Environmental Microbiology*]: http://bit.ly/S5C6ie
[*The ISME Journal - Multidisciplinary Journal of Microbial Ecology*]: http://bit.ly/YgJwEf
[*FEMS Microbiology Ecology*]: http://bit.ly/TXNQku
[*Applied and Environmental Microbiology*]: http://bit.ly/RbpoSa
[*Tufte handouts style*]: http://bit.ly/Vjx3wk