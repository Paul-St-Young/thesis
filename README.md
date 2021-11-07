# thesis

### allow .bib and \bibitem to coexist
1. create .bbl using \bibliographystyle{unsrt}, check that \bibtem in .bbl have no hard-coded citation names in [].
2. include .bbl instead of .bib.

### allow .eps and .pdf to coexist for htlatex
1. Google "pdf htlatex".
2. Modify "myxhtml.cfg" to convert .eps and .pdf to .png.
3. After htlatex, transfer figures along with .html. eg.
  `find papers -name "*.png" | xargs tar -zcvf papers.tgz`

### remove abstract from .bib
biber.exe --tool --configfile=remabs.conf hsolid.bib

Fedora:
texlive-make4ht
texlive-latex
Ubuntu:
textlive-extra-utils
