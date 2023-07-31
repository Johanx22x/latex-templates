# Makefile for LaTeX document with BibTeX

# Replace 'main' with the name of your main .tex file (without the .tex extension)
MAIN = main

all: pdf

pdf:
	latex $(MAIN)
	bibtex $(MAIN)
	latex $(MAIN)
	pdflatex $(MAIN)

clean:
	rm -rf *.aux *.bbl *.blg *.log *.out *.pdf *.toc *.dvi *.lof *.lot

.PHONY: all pdf clean