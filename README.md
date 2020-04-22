<h1 align="center">TourHunter Help Center</h1>

Live: https://help.tourhunter.com

The repository is a part of the [TourHunter Organization](https://github.com/tourhunter-com).

## Code of Conduct

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Contributing

Please read through our [Contributing Guidelines](CONTRIBUTING.md) and [Installation Instructions](INSTALL.md).

## How it works

### Internationalization

Has the following components:

- fields in front matter
- directory structure similar for different languages (i.e. you create files for every translation under their own language directory `/en/_posts/post1`, `/ru/_posts/post1`, etc.)
- config values

### Search

[SimpleJekyllSearch documentation](https://github.com/christian-fei/Simple-Jekyll-Search#usage)

#### Fields in front matter to use in layouts (filtering)

All posts and pages have 2 fields:

- `ref` (effectively unique id of the page or post)
- `lang` (2 letter language code in [ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) format)

And the layouts use these fields to, for example, show only the language already selected by the reader.

#### Directory structure

For every supported language you have a dir:

- `_en/`
- `_ru/`

(Under the hood these are [Jekyll collections](https://jekyllrb.com/docs/collections/), see also: `_config.yml`.

#### Config values

There are a few config files for convenience.

**Jekyll config values**

One - common Jekyll config. The part related to i18n is this:

```ruby
defaults:
 #languages
 -
  scope:
   path: "en"
  values:
   lang: "en"
 -
  scope:
   path: "ru"
  values:
   lang: "ru"
```

This means, that, when you browse files under `en/`, for example, your `site.lang` automatically becomes `en` (and you get all the search results, layouts, etc. for the chosen language).

**i18n configs**

I've put them under `_data/i18n`. They contain translations used in pages, i.e. common lexemes like "Category", section names, etc.

(Your old en.yml, ru.yml, etc.)

Example part of such file:

 ```ruby
main:
  welcomeSection:
    anchor: how
    heading: How can we help?
    p1: Looking for something? Search it here!
```

And these values are used in templates like this:

```ruby
{{site.data.i18n[page.lang].categories.category}}:
```

**Categories config**

Located in `_data/categories.yml`, this is main place to store info about categories. Right now it looks like this:

```ruby
categories:

  - title:
      en: "Getting Started"
      ru: "Начало работы"
    desc:
      en: "Getting started desc from _data/categories.yml"
      ru: "Начало работы... етц"
```

And that's all. Also check `_layouts` directory contents for understanding, how all these vars are used.

## License

This project is open source and available freely under the [MIT license](LICENSE.md).
