## Hammer Buildpack for Heroku

This buildpack allows you to deploy a [Hammer](http://hammerformac.com/) project to Heroku as a static site, served with Nginx.

Repositories are considered a valid Hammer project if they contain a `Build` directory. This directory must be committed to the repository because the Hammer build process cannot be run on the server, only locally.

#### Usage

    $ heroku create --stack cedar --buildpack http://github.com/danpalmer/heroku-buildpack-hammer.git

    $ git push heroku master
    ...
    