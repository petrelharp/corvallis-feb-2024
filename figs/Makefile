SHELL := /bin/bash
.PHONY: figs modeling_figs

figs: modeling_figs mapNN/feems_1.png mapNN/feems_1a.png

modeling_figs: modeling_empty.png \
			   modeling_reality.png \
			   modeling_model_parameters.png \
			   modeling_model_parameters_inverse.png \
			   modeling_parameters_inverse_computer.png

modeling_%.pdf: modeling.ink.svg
	./export-layers-svg.sh $< $@ data $(subst _, ,$*)

include ../rules.mk
