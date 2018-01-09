```bash

$ brew install elixir

$ mix local.hex

$ mix archive.install https://github.com/phoenixframework/archives/raw/master/phx_new.ez

$ mix phx.new blog

We are all set! Go into your application by running:

    $ cd blog

Then configure your database in config/dev.exs and run:

    $ mix ecto.create  (make sure to run postgres server)

Start your Phoenix app with:

    $ mix phx.server

You can also run your app inside IEx (Interactive Elixir) as:

    $ iex -S mix phx.server



# http://localhost:4000/




$  mix phx.gen.html Tests Post posts title:string body:text   # Tests will be a "namespace"

Add the resource to your browser scope in lib/blog_web/router.ex:

    resources "/posts", PostController


Remember to update your repository by running migrations:

    $ mix ecto.migrate



http://localhost:4000/posts




#-------------- pushing to heroku:

$ git init
$ git add .
$ git commit -m 'first commit'


$ touch Procfile
# web: MIX_ENV=prod mix phoenix.server


heroku create spinos-phoenix --buildpack "https://github.com/HashNuke/heroku-buildpack-elixir.git"

# set git remote heroku to https://git.heroku.com/spinos-phoenix.git
heroku git:remote -a spinos-phoenix

git push heroku master





# https://spinos-phoenix.herokuapp.com
# https://spinos-phoenix.herokuapp.com/test


# adding code to my github account
$ git remote add origin git@github.com:brianspinos777/spinos-phoenix.git
$ git push --force
$ git push -u origin master # set upstream
$ git remote show origin
$ git remote -v


```



heroku addons:create heroku-postgresql:hobby-dev
heroku config:set POOL_SIZE=18
mix phoenix.gen.secret # generate secret
heroku config:set SECRET_KEY_BASE="fsfsdhfskdfhsdfsdfsdhfsjdfhsdf"



