SHELL := /bin/bash

%.pdf : %.tex
	latexmk --pdf $*.tex

slideshow.pdf : slideshow.tex \
	regbibliography.bib

clean :
	rm -f slideshow.{aux,bbl,bcf,blg,fdb_latexmk,fls,log,nav,out,run.xml,snm,toc} \
	*~

squeaky : clean
	rm -f slideshow.pdf
