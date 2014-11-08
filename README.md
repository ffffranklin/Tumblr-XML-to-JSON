# spottr-rails 

(previously Tumblr-XML-to-JSON)

This was a helper tool for [Max Wheeler's](http://makenosound.com/) idea to use 
[Mustache](http://mustache.github.com/) to make [Tumblr theme](http://www.tumblr.com/docs/en/custom_themes) 
development much easier. The result is [Tumblr Themr](http://tumblrthemr.icelab.com.au/).

It takes the output of a Tumblr blog filled with dummy content using an XML theme and converts it to JSON that Mustache can use natively.

I mearly updated it to run on heroku for all to use.  Eventually I will be making a more robust version to run on node.js in tandem with weavr (a new way to develop tumblr themes)

## Running Locally

Asumming you have [Ruby](https://www.ruby-lang.org), [Bundler](http://bundler.io) and [Heroku Toolbelt](https://toolbelt.heroku.com) installed on your machine:

```sh
git clone git@github.com:ffffranklin/spottr-rails.git # or clone your own fork
cd spottr-rails
bundle
foreman start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

### Usage

* [http://localhost:5000/content](http://localhost:5000/content) for default dummy data
* [http://localhost:5000/content/daydreamtheme.tumblr.com](http://localhost:5000/content/daydreamtheme.tumblr.com) for your own dummy data

## Deploying to Heroku

```
heroku create
git push heroku master
heroku open
```

## Documentation

For more information about using Ruby on Heroku, see these Dev Center articles:

- [Ruby on Heroku](https://devcenter.heroku.com/categories/ruby)
- [Getting Started with Ruby on Heroku](https://devcenter.heroku.com/articles/getting-started-with-ruby)
- [Getting Started with Rails 4.x on Heroku](https://devcenter.heroku.com/articles/getting-started-with-rails4)
- [Heroku Ruby Support](https://devcenter.heroku.com/articles/ruby-support)
