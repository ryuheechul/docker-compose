.PHONY: bootstrap run

bootstrap:
	docker run --rm -it -w="/bootstrap" -v `pwd`:/bootstrap node:7.7.2-alpine npm init

run:
	docker-compose run app
