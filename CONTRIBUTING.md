# Contributing Guidelines

First off, thanks for taking the time to contribute!

The following is a set of guidelines for contributing to TourHunter, which are hosted in the [TourHunter Organization](https://github.com/tourhunter-com) on GitHub. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Admin interface

This project has admin interface, accessible locally.
Run from command line in the project directory:

```bash
bundle install
```

then start development server: 
```bash
bundle exec jekyll serve
```

and navigate to

```bash
http://localhost:4000/admin
```

to see the content.

## How to add new...
### Article

1. Create new files for each language: `filename.md` in `_posts` directory, i.e. 

    ```bash
    $ touch {en,ru}/_posts/YYYY-MM-DD-new-post.md
    ```
    (Note: post naming format is Jekyll requirement.)

2. Add **front matter** ([Documentation on front matter](https://jekyllrb.com/docs/front-matter/))
Example: 
```
layout: post
title:  "Bienvenue sur Jekyll !"
date:   2016-02-29 09:48:44 +0100
categories: "Marketplace" "Getting Started" (space-separated list of strings)
ref: welcome
lang: fr
```

3. Write the post.

[Official Jekyll doc on Posts](https://jekyllrb.com/docs/posts/)

### Page

Basically all the same actions as for `_posts`, just `_pages` subdirectory and slightly other fields in front matter.

### Category
1. Add name and description into `_data/categories.yml`
2. Create new markdown file in `category` dir (using slug for name, i.e. "Getting Started" -> "getting-started.md")

    ```bash
    $ touch {en,ru}/category/new-category-slug.md
    ```

3. Front matter should contain the following fields:
    ```
    layout: category
    category: getting-started
    permalink: /category/getting-started
    ```

3. Regenerate the site.
Something similar to:

    ```bash
    bundle exec jekyll build
    ```

And we're golden.
