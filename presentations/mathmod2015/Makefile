TEXINPUTS:=":tex/::"
export TEXINPUTS

img/%.tikz.svg : tex/%.tikz.tex tex/modml.sty
		pdflatex --halt-on-error --interaction=scrollmode --output-directory=tmp/ $< 
		pdflatex --halt-on-error --interaction=scrollmode --output-directory=tmp/ $< 
		pdf2svg tmp/$*.tikz.pdf $@

all: img/circuit-scale.tikz.svg img/circuit.tikz.svg img/matrix.tikz.svg \
	img/pendulum-equations.tikz.svg \
	img/pendulum-equations-sorted.tikz.svg \
	img/pendulum-equations-reduced.tikz.svg \
	img/sigma-matrix-pendulum.tikz.svg \
	img/sigma-matrix-circuit.tikz.svg \
	img/sigma-matrix-circuit-component.tikz.svg \
	img/sigma-matrix-circuit-compressed.tikz.svg \
	img/sigma-matrix-circuit-opening.tikz.svg \
	img/sigma-matrix-circuit-open.tikz.svg \
	img/sigma-matrix-circuit-open2.tikz.svg \
	img/sigma-matrix-circuit-closing.tikz.svg \
	img/sigma-matrix-compressed-circuit.tikz.svg \
	img/circuit-code.tikz.svg





