.PHONY: index2.html index2.pdf
.SUFFIXES: .qmd .html


LaTeX = pdflatex
LaTeX = xelatex
QUARTO = quarto



main: 202510-proteoBench.html
	open $<

deploy: 202510-proteoBench.html
	scp 202510-proteoBench.html r35:~/WWW/ProteoBenchChallenge/$<

.qmd.html:
	$(QUARTO) render $<

clean:
	$(RM) *.pdf *.html
