TARGET		= cv_dev
TEMPLATES 	= Preamble_CV.tex
FLAGS  		= --interaction=nonstopmode

$(TARGET).pdf : $(TARGET).tex $(TEMPLATES)
	pdflatex $(TARGET).tex $(FLAGS) -output-directory=build 1> /dev/null
	cp $(TARGET).pdf ~/Downloads/DanielSanchezCV.pdf

open: $(TARGET).pdf
	evince $(TARGET).pdf

clear:
	rm -f *.aux *.log *.out *.pdf
	clear && exa --color=always
