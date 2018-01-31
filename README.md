## Sinatra Example Blog

This is a good example of structuring a Sinatra app.
Feel free to clone it, browse the source, customize it
and use it as your own blog.

Good examples of the following:

* Using Sinatra routes as middleware
* GZip and caching
* RSS feed of posts
* Sprockets and asset management
* Markdown and Erb
* Unicorn and Heroku
* Stylus

Demo here http://sinatra-example-blog.herokuapp.com

## Running

### pre-install directions
install memcached if you don't have it, to support this app

Using Mac, run these commands:
`brew install memcached`
`brew services start memcached`

### install directions
    bundle install
    thin start

## Heroku 123

    git clone git@github.com:maccman/sinatra-blog.git
    cd sinatra-blog

    heroku create myblog
    heroku labs:enable user-env-compile
    heroku addons:add memcachier:dev

    git push heroku master
