TARGETS = main

LATEX	= xelatex
BIBTEX	= bibtex

all:    $(TARGETS) debug

$(TARGETS):
		$(LATEX) $@
		-$(BIBTEX) $@ > $(BIBTEX)_out.log
		$(LATEX) $@
		$(LATEX) $@
		$(LATEX) $@

debug:
		-grep Warning *.log
clean:  
		rm -f images/*.aux images/*.log *.snm *.nav *.out *.toc *.aux *.bbl *.blg *.log *.dvi *.bak *~ $(TARGETS:%=%.pdf)
