filename=semp

all:
	"/Library/TeX/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex && open ${filename}.pdf

view: pdf
	open ${filename}.pdf

pdf:
	"/Library/TeX/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex && "/Library/TeX/texbin/pdflatex" -synctex=1 -interaction=nonstopmode "${filename}".tex

clean:
	rm -f ${filename}.{ps,pdf,log,aux,out,dvi,bbl,blg} && rm chapter/*.aux
