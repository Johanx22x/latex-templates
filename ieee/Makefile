FILES = src/*.md \

OUTPUT = build

FLAGS = --bibliography=lib/bibliography.bib \
		--from=markdown \
		--to=latex \
		--template=lib/template.latex \
		--csl=lib/bibliography.csl \
		--filter=pandoc-crossref \
		--citeproc \
		--metadata-file=metadata.yaml \
		-s \
		-t pdf

all: pdf

--template=lib/template.latex

pdf:
	pandoc -o $(OUTPUT)/paper.pdf $(FLAGS) $(FILES)

clean:
	rm build/*

