# BIBEMME #
## Biblatex styles for journals of environmental microbiology and microbial ecology ##

All styles are designed to work with [biblatex](http://bit.ly/Sn6Bjx) 2.3 and above alongside with [biber](http://bit.ly/SjJLe6).  
In constructing the styles I referred to the author guidelines of each journal but also to publications from latest issues, since there are occasional conflicts or missing guidelines regarding some types of sources or special cases. Each style defines explicitly the formatting of only the following bibtex reference types: article, book and incollection. Other types are too rare and in any case are not formally described in the author guidelines.


** Disclaimer **
This project as a whole and each style in particular are under continuous development and might therefore contain mistakes or bugs. 

Copyright (C) 2012 Roey Angel 
<angel@mpi-marburg.mpg.de>

THIS PROGRAM COMES AS IS WITH ABSOLUTELY NO WARRANTY.
This software is distributed under the terms of the GNU General Public License Version 3.

This project was inspired by Timothée Poisot's [ecobiblatex](http://bit.ly/10TlcHw) and I used his geb.bbx as a template.

### Usage: ###
Please refer to .bbx file of each individual style for specific instructions.  

1. Place the .bbx and .cbx files in your tex path (e.g. `$TEXMFLOCAL/tex/latex/biblatex` in linux) and add the following to the preamble:  
`\usepackage[style=STYLE_NAME, natbib=true, backend=biber]{biblatex}`  
`\addbibresource{YOUR_BIB_FILE.bib}`  
The style and .bib source names should, of course, be replaced by the desired citation style and your personal bibtex collection file.  
2. For styles requiring journal name abbreviations (all styles at the moment), the file `JourAbs.map` or a link to it must be placed withing the same directory as the LaTeX document.  
3. Add a bibliography list in the document using: `\printbibliography[sorting=STYLESPECIFICSORT]`. Typically the references should be sorted using `\printbibliography[sorting=nyt]` but note that some styles might require a different sorting scheme (e.g. emi).

## Currently available styles ##

1. emi:     [*Environmental Microbiology*](http://bit.ly/S5C6ie)
2. ismej:   [*The ISME Journal - Multidisciplinary Journal of Microbial Ecology*](http://bit.ly/YgJwEf)
3. femsme:  [*FEMS Microbiology Ecology*](http://bit.ly/TXNQku)
4. aem:     [*Applied and Environmental Microbiology*](http://bit.ly/RbpoSa) - *coming soon*