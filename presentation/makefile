texFile:=$(shell ls *.tex|head -1|sed 's/.tex//')
all: ${texFile}.pdf
${texFile}.pdf: ${texFile}.tex beamerthemeSingapore2.sty
	pdflatex -output-directory tmp ${texFile}.tex
	pdflatex -output-directory tmp ${texFile}.tex
	cp tmp/${texFile}.pdf .

