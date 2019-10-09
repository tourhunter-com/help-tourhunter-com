# TourHunter Help Center

## Features
- i18n (multiple languages)

## How to add new...
### Article

1. Create new files for each language: `filename.md` in `_articles` directory. 
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

[Official Jekyll doc on Posts](https://jekyllrb.com/docs/posts/)

### Page
[//] # wx: todo

### Category
1. Add name and description into `_data/categories.yml`
2. Create new markdown file in `_category` dir (using slug for name, i.e. "Getting Started" -> "getting-started.md"), front matter should contain the following fields:
```
layout: category
category: getting-started
permalink: /category/getting-started
```
3. Regenerate the site

------

# Development

## How to add new...

### Lexeme
1. `_data/i18n/%lang%.yml` - add new lexeme into the hierarchy;
2. Reference like this: `site.data.i18n[page.lang].place.in.the.hierarchy.your_lexeme`

### Support for multiple languages
It works without any special plugins. Here's how:

*In article*: front matter contains 2 mandatory fields: `ref` and `lang`. 

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/tourhunter-com/help/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/tourhunter-com/help/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
