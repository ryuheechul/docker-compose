.PHONY: mix iex shell

elixir-iex:
	docker-compose run elixir iex
elixir-shell:
	docker-compose run elixir bash
iex:
	docker-compose run app iex
mix:
	echo "'bin/docker/mix {args}' instead"
shell:
	docker-compose exec app bash
run-f:
	docker-compose up
