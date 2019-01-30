Heroku Ruby Jekyll Buildpack for Gitlab CI
============================

Heroku Ruby Jekyll Buildpack is a fork of Heroku's [official Ruby buildpack](https://github.com/heroku/heroku-buildpack-ruby) with added support for generating static [Jekyll](https://github.com/mojombo/jekyll) sites during the build/deployment stage.

With this [buildpack](http://devcenter.heroku.com/articles/buildpacks) you no longer need pre-build the site or commit the _site build directory to your repo. This simplifies the deployment process and keeps the repo clean. All of the standard Ruby tools are maintained in this buildpack, so you can take full advantage of Rack middleware and other useful tools from the Ruby ecosystem.


## Usage

    heroku create --buildpack http://github.com/leemp/heroku-buildpack-ruby-jekyll.git

or add this buildpack to your current app

    heroku config:add BUILDPACK_URL=http://github.com/leemp/heroku-buildpack-ruby-jekyll.git

Create a Ruby web app with dependencies managed by [Bundler](http://gembundler.com/) and a Jekyll site. [Heroku-Jekyll-Hello-World](https://github.com/burkemw3/Heroku-Jekyll-Hello-World) can be used as a sample starter.
