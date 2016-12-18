TARG=example

SRC = $(shell find . -name "*.tex") ../dojin-style.sty

$(TARG).pdf: $(SRC)
	lualatex --halt-on-error $<

clean:
	rm -rf *.aux *.bbl *.blg *.dvi *.idx *.ilg *.ind *.lof *.log *.toc *.pdf
