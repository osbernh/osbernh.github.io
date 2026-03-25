# Maintaining the Website

This website uses the `academicpages` Jekyll scaffold. Most maintenance is done by editing Markdown files and then pushing changes to GitHub.

## 1. Start from the website folder

```bash
cd /Users/osbern/Documents/Website_Academic/osbernh.github.io
```

## 2. Preview locally

If Ruby is already set up:

```bash
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

## 3. Edit the homepage and main profile

- Home page: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_pages/about.md`
- Site-wide profile/sidebar info: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_config.yml`
- Top navigation: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/_data/navigation.yml`

## 4. Add or edit blog posts

Blog posts live in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_posts/`

Filename format:

`YYYY-MM-DD-title.md`

Example:

```md
---
title: "My New Post"
date: 2026-03-25
permalink: /posts/my-new-post/
tags:
  - research
  - methods
---

Write your post here in Markdown.
```

## 5. Add or edit publications

Publication entries live in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_publications/`

Each publication is one Markdown file with a YAML header. Copy an existing file and edit the title, venue, citation, excerpt, and date.

## 6. Add or edit teaching entries

Teaching entries live in:

`/Users/osbern/Documents/Website_Academic/osbernh.github.io/_teaching/`

Each teaching item is one Markdown file.

## 7. Update CV and files

- CV download file: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/files/CV.pdf`
- Portrait image: `/Users/osbern/Documents/Website_Academic/osbernh.github.io/images/Portrait.jpg`

If you replace either file, keep the same filename so the links keep working.

## 8. Publish to GitHub

After checking the site locally:

```bash
git add .
git commit -m "Update website content"
git push
```

GitHub Pages will rebuild the site automatically.

## 9. Basic Markdown you will use most often

```md
# Big heading
## Section heading

This is a paragraph.

- Bullet one
- Bullet two

[Link text](https://example.com)

**Bold text**
*Italic text*
```

## 10. Safe editing habit

1. Run `bundle exec jekyll serve`
2. Edit one file
3. Refresh the browser
4. When it looks right, run `git add . && git commit -m "..." && git push`
