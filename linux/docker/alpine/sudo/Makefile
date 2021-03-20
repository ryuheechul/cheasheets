.PHONY: test
test: build
	docker run --rm -it my-cheatsheets-alpine-sudo sh -c 'whoami && sudo ls -lah /root'

.PHONY: run
run: build
	docker run --rm -it my-cheatsheets-alpine-sudo

.PHONY: build
build:
	docker build . -t my-cheatsheets-alpine-sudo
