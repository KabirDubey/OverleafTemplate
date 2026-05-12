ROOT = main
BUILD = build

.PHONY: all pdf watch clean open skim

all: pdf

pdf:
	latexmk -pdf -xelatex -bibtex $(ROOT).tex

watch:
	latexmk -pdf -xelatex -bibtex -pvc $(ROOT).tex

open:
	open $(BUILD)/$(ROOT).pdf

skim:
	open -a Skim $(BUILD)/$(ROOT).pdf

clean:
	latexmk -C $(ROOT).tex
	rm -rf $(BUILD)
