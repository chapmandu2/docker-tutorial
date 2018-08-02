help:
	@echo Makefile commands:
	@echo
	@echo help: print this help message and exit
	@echo build: build the docker image
	@echo run: run the docker image

build:
	docker build . --tag='phil-r4'

run:
	docker run -it --rm phil-r4

run-data:
	docker run -it --rm -v ~/Documents:/localdata phil-r4
