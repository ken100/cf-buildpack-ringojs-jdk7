Heroku buildpack: RingoJS
========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for [RingoJS](http://ringojs.org/) apps.

Usage
-----

Example usage:

    $ ls
    app.js

    $ heroku create --stack cedar --buildpack https://github.com/jockm/heroku-buildpack-ringojs-jdk7.git
	
	$ git push heroku master

    -----> Heroku receiving push
    -----> Fetching custom build pack... done
    -----> RingoJS app detected
    -----> Installing RingoJS..... done

The buildpack will detect your app as a RingoJS project if it has a file called app.js. If you don't provide a Procfile, the build pack will default to launching your app with `ringo app.js`
