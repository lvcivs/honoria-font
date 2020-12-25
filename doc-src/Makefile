.PHONY: pdf view-pdf

PROJECT_NAME = honoria

# shall we stop latex when encoutering an error?
INTERACTION = errorstopmode

# choose PDF viewer
PDFVIEWER = atril

all: view-pdf

pdf:
	xelatex -interaction=$(INTERACTION) -no-pdf -papersize=a4 $(PROJECT_NAME).tex
	xelatex -interaction=$(INTERACTION) -papersize=a4 $(PROJECT_NAME).tex


view-pdf: pdf
	 $(PDFVIEWER) $(PROJECT_NAME).pdf &

clean:
	rm -f  $(PROJECT_NAME).aux
	rm -f  $(PROJECT_NAME).log
	rm -f  $(PROJECT_NAME).xdv
	rm -f $(PROJECT_NAME).bcf

