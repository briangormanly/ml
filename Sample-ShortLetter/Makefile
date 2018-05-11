filename=Letter

pdf: ps
		ps2pdf ${filename}.ps
		rm -f ${filename}.{log,aux,out,bbl,blg}

ps:	dvi
		dvips ${filename}.dvi

dvi:
		latex ${filename}.tex
			latex ${filename}.tex
