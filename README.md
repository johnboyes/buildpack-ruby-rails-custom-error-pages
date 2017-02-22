# Heroku buildpack for copying html files from `public/assets` to `public` on deploy
(e.g. custom error pages in a rails app that have been precompiled by the rails asset pipeline)

This buildpack is intended for use after the regular [ruby-buildpack].

# Usage

If you are using the default buildpack, manually set your buildpack to Heroku's default Ruby buildpack

```
heroku buildpacks:set https://github.com/heroku/heroku-buildpack-ruby
```

Append the buildpack-ruby-rails-custom-error-pages to your buildpack list:

```
heroku buildpacks:add https://github.com/johnboyes/buildpack-ruby-rails-custom-error-pages
```

# License

MIT, see the [LICENSE.md](LICENSE.md) file.
