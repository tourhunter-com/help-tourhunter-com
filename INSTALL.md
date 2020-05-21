# Installation

Please read through our [Contributing Guidelines](CONTRIBUTING.md).

## General setup

- Install [Ruby](https://www.ruby-lang.org/en/documentation/installation/)
- Install [Bundler](https://bundler.io)
- Install [Jekyll](https://jekyllrb.com/docs/installation/)

Before you start, install dependencies:
```
bundle install
```

Start development server:
```
bundle exec jekyll serve
```

Open your browser:
- http://localhost:4000 - website content.
- http://localhost:4000/admin - admin interface.

In case you need to rebuild the website:
```
bundle exec jekyll build
```

In case you need to update dependencies:
```
bundle update listen
```

## Additional information

- https://help.github.com/en/articles/testing-your-github-pages-site-locally-with-jekyll
