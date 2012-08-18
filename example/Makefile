TARG=example

SRC       = $(shell find . -name "*.tex") ../dojin-style.sty
TEX_FLAGS = -halt-on-error -kanji=utf8

$(TARG).pdf: $(TARG).dvi
	dvipdfmx -p jisb5 -o $@ $<

$(TARG).dvi: $(SRC)
	platex $(TEX_FLAGS) $(TARG).tex
	platex $(TEX_FLAGS) $(TARG).tex

clean:
	rm -rf *.aux *.bbl *.blg *.dvi *.idx *.ilg *.ind *.lof *.log *.toc *.pdf
