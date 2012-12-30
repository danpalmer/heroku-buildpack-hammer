## Hammer Buildpack for Heroku

This buildpack allows you to deploy a [Hammer](http://hammerformac.com/) project to Heroku as a static site, served with Nginx.

Repositories are considered a valid Hammer project if they contain a `Build` directory. This directory must be committed to the repository because the Hammer build process cannot be run on the server, only locally.

#### Usage

    $ heroku create --stack cedar --buildpack http://github.com/danpalmer/heroku-buildpack-hammer.git

    $ git push heroku master
    ...
    -----> Downloading Nginx Sources
    -----> Extracting Nginx Sources
    -----> Configuring
    -----> Compiling
    -----> Installing
    -----> Creating Boot Script


#### Credits

Tips on the general process of using Nginx on Heroku taken from mchung/heroku-buildpack-nginx by @mchung.

