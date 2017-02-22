# Heroku buildpack for copying html files from `public/assets` to `public` on deploy

## Example use case:
allows you to serve custom error pages in a rails app that have been precompiled by the
rails asset pipeline as static files.

See https://medium.com/@tair/custom-error-pages-in-rails-you-re-doing-it-wrong-ba1d20ec31c0

## Set up

This buildpack is intended for use after the regular [ruby-buildpack].

If you are using the default buildpack, manually set your buildpack to Heroku's default
Ruby buildpack

```
heroku buildpacks:set heroku/ruby
```

Append the buildpack-ruby-rails-custom-error-pages to your buildpack list:

```
heroku buildpacks:add https://github.com/johnboyes/buildpack-ruby-rails-custom-error-pages
```

More info: [Heroku Dev Center article on multiple buildpacks]

# License

MIT, see the [LICENSE.md](LICENSE.md) file.

[ruby-buildpack]:https://github.com/heroku/heroku-buildpack-ruby
[Heroku Dev Center article on multiple buildpacks]:https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app
