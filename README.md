# Discuss

This is my coursework for the Udemy course: ['The Complete Elixir and Phoenix Bootcamp'](https://www.udemy.com/the-complete-elixir-and-phoenix-bootcamp-and-tutorial/)

## To Download
  
  At a shell or command prompt:
  ```
  git clone https://github.com/pursuitky/discuss.git
  cd discuss
  git checkout section13
  ```

## To start your Phoenix app:

  ### Section 11 branch (and onward):
  Create a Dicuss OAuth App in Github.
  Create a secrets file named "config.secret.exs" in the /config folder of the app.
  ```elixir
  use Mix.Config

  config :ueberauth, Ueberauth.Strategy.Github.OAuth,
  client_id: "<Github client id key here>",
  client_secret: "<Github client secret key here>"
  ```
  
  Create another secrets file named "dev.secret.exs" in the /config folder of the app.
  ```elixir
  use Mix.Config

  # Configure your database
  config :discuss, Discuss.Repo,
    adapter: Ecto.Adapters.Postgres,
    username: "<Your DB username>",
    password: "<Your DB password>",
    database: "discuss_dev",
    hostname: "localhost",
    pool_size: 10
  ```

  ### For all branches:
  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.create && mix ecto.migrate`
  * Install Node.js dependencies with `npm install`
  * Start Phoenix endpoint with `mix phoenix.server`

Now you can visit [`localhost:4000`](http://localhost:4000) from your browser.

Ready to run in production? Please [check our deployment guides](http://www.phoenixframework.org/docs/deployment).

## Learn more

  * Official website: http://www.phoenixframework.org/
  * Guides: http://phoenixframework.org/docs/overview
  * Docs: https://hexdocs.pm/phoenix
  * Mailing list: http://groups.google.com/group/phoenix-talk
  * Source: https://github.com/phoenixframework/phoenix
