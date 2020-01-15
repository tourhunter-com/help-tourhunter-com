# Contributing Guidelines

First off, thanks for taking the time to contribute!

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).

## How to add new...

### Article

1. Create new files for each language: `filename.md` or `file_name.md` in `_articles-lang` directory, i.e.

    ```bash
    _articles-en/article_name.md
    ```

2. Add **front matter** ([Documentation on front matter](https://jekyllrb.com/docs/front-matter/))

Example:

```
layout: article
title:  "Article name"
date:   2016-02-29 09:48:44 +0100
excerpt: "Part of a post"
category: marketplace
tags:
- related-article-name1
- related-article-name2
lang: en
ref: article-name
permalink: "/en/:name/"
```

or

```
layout: article
title:  Название статьи
date:   2019-04-11 12:32 +0100
excerpt: "Part of a post"
categories:
- getting-started
- marketplace
- agents
lang: ru
ref: article-name
permalink: "/ru/:name/"
```

3. Put links inside the article on other articles if it's necessary ([Documentation on links](https://jekyllrb.com/docs/liquid/tags/#links)). All links should be relative and not absolute. 

4. Add images or gif-animations ([Documentation on images](https://jekyllrb.com/docs/posts/#including-images-and-resources)). There should not be unnecessary actions and movements of the mouse in the image (gif-animation), only what relates to the explanation. All images and gif-animations shoul be in high resolution.

5. The format of images must be png or jpeg. The width of the images and gif-animations should not exceed 750 px.

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
