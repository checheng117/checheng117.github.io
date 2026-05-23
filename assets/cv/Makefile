LATEXMK ?= latexmk
TEX := cv.tex
JOB := CV_Che_CHENG
PDF := $(JOB).pdf

.PHONY: all clean distclean

all: $(PDF)

$(PDF): $(TEX)
	$(LATEXMK) -pdf -interaction=nonstopmode -halt-on-error -jobname=$(JOB) $(TEX)

clean:
	$(LATEXMK) -c -jobname=$(JOB) $(TEX)
	rm -f $(JOB).aux $(JOB).fdb_latexmk $(JOB).fls $(JOB).log $(JOB).out $(JOB).synctex.gz

distclean: clean
	rm -f $(PDF)
