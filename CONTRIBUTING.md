# Contributing Guidelines

First off, thanks for taking the time to contribute!

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Getting Started

When contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the core team before making a change.

- Make sure you have a [GitHub account](https://github.com/login).
- Submit a GitHub issue for your issue if one does not already exist.
  - A issue is not necessary for trivial changes.
- Create a new branch (preferred, if it is available) or [fork](https://help.github.com/en/articles/working-with-forks) the repository on GitHub.
- Make your change. Add tests for your change. Make the tests pass.
- Create a [pull request](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork) to the repository.

### Tips and tricks for using the Git

- [GitHub Cheat Sheet](https://github.com/tiimgreen/github-cheat-sheet)
- [git-tips](https://github.com/git-tips/tips)

## How to add new...

### Article

1. Create new files for each language: `filename.md` or `file_name.md` in `_articles-lang` directory, i.e.

    ```
    _articles-en/article_name.md
    ```

2. Add **front matter** ([Documentation on front matter](https://jekyllrb.com/docs/front-matter/))

Example:

```
title:  Article name
layout: article
date:   2016-02-29 09:48:44 +0100
excerpt: "Part of a post"
category: bookings
subcategories:
	bookings: transfer-view
tags:
- related-article-name1
- related-article-name2
lang: en
permalink: "/en/:name/"
ref: article-name
```

or

```
title:  Название статьи
layout: article
date:   2019-04-11 12:32 +0100
excerpt: "Part of a post"
category: getting-started
lang: ru
permalink: "/ru/:name/"
ref: article-name
```

3. Put links inside the article on other articles if it's necessary ([Documentation on links](https://jekyllrb.com/docs/liquid/tags/#links)). All links should be relative and not absolute, i.e.

    ```
    ![file_name1](/assets/images/file_name1.png)
    ```

4. Add images or gif-animations ([Documentation on images](https://jekyllrb.com/docs/posts/#including-images-and-resources)): `filename1.png` or `file_name2.jpeg` in `assets/images` directory, i.e.

    ```
    assets/images/file_name1.jpeg
    ```

There should not be unnecessary actions and movements of the mouse in the image (gif-animation), only what relates to the explanation. All images and gif-animations shoud be in high resolution.

5. The format of images must be png or jpeg.

### Category

1. Add name and description into `_data/categories.yml`

2. Create new markdown file in `_lang/category` dir (using slug for name, i.e. "Getting Started" -> "getting-started.md")

    ```
    $ touch _{en,ru}/category/new-category-slug.md
    ```

3. Front matter should contain the following fields:
    ```
    layout: category
    category: getting-started
    permalink: /category/getting-started
    ```

4. Change description into `_data/categories.yml` for add subcategory, i.e.

    ```
  category-name:
    title:
      en: "Name of category"
      ru: "Название категории"
    desc:
      en: "Description text."
      ru: "Текст описания."
    subcategories:
      subcategory-name:
        en: "Name of subcategory"
        ru: "Название подкатегории"
    ```

5. Rebuild the website:
    ```
    bundle exec jekyll build
    ```

### Lexeme

1. `_data/i18n/%lang%.yml` - add new lexeme into the hierarchy;

2. Reference like this: `site.data.i18n[page.lang].place.in.the.hierarchy.your_lexeme`

## Additional information

- https://help.github.com/en/articles/adding-content-to-your-github-pages-site-using-jekyll
