SOURCE:=$(wildcard pb*.tex)
DVIFILES:=$(SOURCE:%.tex=%.dvi)
PDFFILES:=$(SOURCE:%.tex=%.pdf)

all: $(PDFFILES)

%.pdf: %.dvi
	dvipdfmx $< 

%.dvi: %.tex
	latex $<
	latex $<
	latex $<

clean:
	rm -fv *~ *.log *.aux *.snm *.toc *.out *.nav *.dvi *.pdf *.pdf
