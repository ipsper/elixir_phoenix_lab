# Elixir phoenix lab

Doing a lab using elixir and phoenix

# Documentastions

[elixir](https://elixir-lang.org/)
[phoenix](https://www.phoenixframework.org/)

# Precondisions

## Precondisions ubuntu

```
[ $(elixir --version | grep -c Elixir) -eq 1 ] && echo "Installed"
```

if Installed jump to Phoenix
[install elixir](https://elixir-lang.org/install.html)

## install elixir on ubuntu

```
sudo add-apt-repository ppa:rabbitmq/rabbitmq-erlang
sudo apt update
sudo apt install elixir erlang-dev erlang-xmerl
```

## install elixir on mac

```
brew install elixir


brew install postgresql


```

# Phoenix

# install Phoenix

```
mix archive.install hex phx_new
```

## install hello demo

```
mix phx.new hello
```

We are almost there! The following steps are missing:

    $ cd hello

Then configure your database in config/dev.exs and run:

    $ mix ecto.create
    `
    Compiling 15 files (.ex)

warning: defining a Gettext backend by calling

    use Gettext, otp_app: ...

is deprecated. To define a backend, call:

    use Gettext.Backend, otp_app: :my_app

Then, instead of importing your backend, call this in your module:

    use Gettext, backend: MyApp.Gettext

lib/hello_web/gettext.ex:23: HelloWeb.Gettext (module)

Generated hello app

16:51:10.243 [error] Postgrex.Protocol (#PID<0.436.0>) failed to connect: \*\* (DBConnection.ConnectionError) tcp connect (localhost:5432): connection refused - :econnrefused

16:51:10.250 [error] Postgrex.Protocol (#PID<0.442.0>) failed to connect: ** (DBConnection.ConnectionError) tcp connect (localhost:5432): connection refused - :econnrefused
** (Mix) The database for Hello.Repo couldn't be created: killed

    `

Start your Phoenix app with:

    $ mix phx.server

You can also run your app inside IEx (Interactive Elixir) as:

    $ iex -S mix phx.server
