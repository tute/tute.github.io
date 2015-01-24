pdflatex:
	pdflatex Relatos_de_distintos_viajes.tex
	if [ -x /usr/bin/evince ]; then evince Relatos_de_distintos_viajes.pdf; else open Relatos_de_distintos_viajes.pdf; fi &

clean:
	rm -f *.toc *.log *.aux *.out *.pdf
