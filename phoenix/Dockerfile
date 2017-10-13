FROM elixir:1.5.2
# RUN wget -qO- https://deb.nodesource.com/setup_4.x | bash -
# RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs

RUN mix local.hex --force
# RUN mix archive.install --force https://github.com/phoenixframework/archives/raw/master/phoenix_new.ez
RUN mix archive.install --force https://github.com/phoenixframework/archives/raw/master/phx_new.ez
RUN mix local.rebar --force

RUN mkdir -p /code
WORKDIR /code

COPY app/mix.exs /code/mix.exs
COPY app/mix.lock /code/mix.lock

RUN yes | mix deps.get
