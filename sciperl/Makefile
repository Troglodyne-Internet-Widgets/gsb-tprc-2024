.PHONY: deps
deps:
	sudo apt-get install latexmk texlive-latex-extra texlive-science texlive-extra-utils texlive-bibtex-extra poppler-utils

.PHONY: all
all: clean
	latexmk -pdf
	pdf2html paper.pdf

.PHONY: clean
clean:
	latexmk -C
	rm paper.bib paper.bbl; /bin/true

