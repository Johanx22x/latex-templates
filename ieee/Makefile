FILES = src/*.md \

OUTPUT = build

FLAGS = --bibliography=lib/bibliography.bib \
		--from=markdown \
		--to=latex \
		--template=lib/template.tex \
		--csl=lib/bibliography.csl \
		--filter=pandoc-crossref \
		--citeproc \
		--metadata-file=metadata.yaml \
		-s \
		-t pdf

all: pdf

--template=lib/template.tex

pdf:
	pandoc -o $(OUTPUT)/paper.pdf $(FLAGS) $(FILES)

clean:
	rm build/*

