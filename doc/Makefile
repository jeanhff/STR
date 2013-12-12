FILE =Final

LATEX_EXECUTABLE=latex
LATEX_VISUALIZATION=evince
LATEX_EXTENSION=ps


all: ${FILE}.tex
	#make clean
	${LATEX_EXECUTABLE} ${FILE}.tex
	dvips ${FILE}.dvi
	ps2pdf ${FILE}.${LATEX_EXTENSION}
	#make clean
clean:
	rm -f *.log *.aux *.bbl *.blg *.dvi *.lot *.toc *.lof *.out *~ *.ps  

see: all
	${LATEX_VISUALIZATION} ${FILE}.pdf &

