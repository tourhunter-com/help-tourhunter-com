# Contributing Guidelines

First off, thanks for taking the time to contribute!

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).

## How to add new...

### Article

1. Create new files for each language: `filename.md` in `_lang` directory, i.e.

    ```bash
    $ touch _{en,ru}/article_name.md
    ```

2. Add **front matter** ([Documentation on front matter](https://jekyllrb.com/docs/front-matter/))
Example:
```
layout: article
title:  "Bienvenue sur Jekyll !"
date:   2016-02-29 09:48:44 +0100
categories: "Marketplace" "Getting Started" (space-separated list of strings)
ref: welcome
lang: fr
```

3. Write the article.


### Category
1. Add name and description into `_data/categories.yml`
2. Create new markdown file in `_lang/category` dir (using slug for name, i.e. "Getting Started" -> "getting-started.md")

    ```bash
    $ touch _{en,ru}/category/new-category-slug.md
    ```

3. Front matter should contain the following fields:
    ```
    layout: category
    category: getting-started
    permalink: /category/getting-started
    ```

3. Rebuild the website:
    ```
    bundle exec jekyll build
    ```

### Lexeme
1. `_data/i18n/%lang%.yml` - add new lexeme into the hierarchy;
2. Reference like this: `site.data.i18n[page.lang].place.in.the.hierarchy.your_lexeme`

## Additional information

- https://help.github.com/en/articles/adding-content-to-your-github-pages-site-using-jekyll
