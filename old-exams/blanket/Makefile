ID=$(shell pwd | xargs basename)

all:
	rm -rf dist
	mkdir -p dist/$(ID)
	python generate.py
	cp input.txt dist/$(ID)
	cp verify.py dist/$(ID)
	cp verilib.py dist/$(ID)
	cp assignment.md dist/$(ID)

test:
	python generate.py
	python solution.py > output.txt
	DIAG= python verify.py
