# Academic Website

This repository contains a simple Jekyll academic website for Osbern Huang, built from the CV files in this workspace and organized for easy maintenance.

## What is included

- A lightweight Jekyll site scaffold that works well with GitHub Pages
- Content stored in `_data/*.yml` so updates usually mean editing structured data instead of HTML
- Separate pages for home, research, publications, teaching, and CV
- `[placeholder]` markers where the CV did not provide enough information

## Quick edits

- Update profile and links in `/Users/osbern/Documents/Website_Academic/_data/profile.yml`
- Update publications in `/Users/osbern/Documents/Website_Academic/_data/publications.yml`
- Update projects in `/Users/osbern/Documents/Website_Academic/_data/projects.yml`
- Update experience in `/Users/osbern/Documents/Website_Academic/_data/experience.yml`

## GitHub Pages publishing

1. Create a GitHub repository.
2. Upload all files in this folder to the repository root.
3. If the repository will be a project site, update `url` and keep `baseurl` in `/Users/osbern/Documents/Website_Academic/_config.yml` aligned with the repository name.
4. In GitHub, open `Settings -> Pages`.
5. Set the source to `GitHub Actions`, or if you prefer native Jekyll builds, use the default Pages build if available for your repo setup.
6. Once published, replace the `[placeholder]` links in `/Users/osbern/Documents/Website_Academic/_data/profile.yml`.

## Local preview

If Ruby and Bundler are available:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

## Notes

- The repository currently includes the original `CV.pdf` and `CV.zip`.
- The site is ready for upload, but local build verification depends on installing Jekyll and the GitHub Pages gem in the environment.
