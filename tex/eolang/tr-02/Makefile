all: report.pdf spell qc

install:
	gem install texsc
	gem install texqc

fast:
	pdflatex --shell-escape report.tex

qc:
	texqc report

spell:
	texsc *.tex

clean:
	rm -rf *.aux *.bbl *.bcf *.blg *.fdb_latexmk *.fls *.log *.run.xml *.pdf *.out
	rm -rf _minted-article

%.pdf: %.tex main.bib *.tex
	latexmk -pdf $<
