filename=thesis

all:
	"/usr/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex && open ${filename}.pdf

view: pdf
	open ${filename}.pdf

pdf:
	"/usr/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex && "/usr/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex

clean:
	rm -f ${filename}.{ps,pdf,log,aux,out,dvi,bbl,blg}
