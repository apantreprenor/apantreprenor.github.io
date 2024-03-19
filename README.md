
# Instructions

To run the project locally, navigate to the project directory and run:

```
bundle install
``` 

To start the Jekyll local development server.

```
bundle exec jekyll serve
bundle exec jekyll serve --livereload
``` 

To build static content

```
jekyll build
```

Clean up your jekyll build and cache

```
bundle exec jekyll clean
```

Issues:
---

Edit the Gemfile.lock and remove the -x64-mingw32 for eventmachine

```
bundle config set install.eventmachine --platform=ruby
bundle config set install.ffi --platform=ruby
gem install eventmachine --platform ruby
```

gemfile.lock

```
gem install eventmachine --platform ruby
```