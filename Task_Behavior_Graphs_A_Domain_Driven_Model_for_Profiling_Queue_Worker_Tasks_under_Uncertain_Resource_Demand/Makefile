PAPER=main

.PHONY: all pdf clean distclean

all: pdf

pdf:
	latexmk -pdf $(PAPER).tex

clean:
	latexmk -c

distclean:
	latexmk -C
	rm -f $(PAPER).bbl
