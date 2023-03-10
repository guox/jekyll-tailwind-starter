---
title: A template for build and deploy Jekyll+Tailwindcss on Github Pages
lang: en
permalink: /en/
---

> Since [GitHub Pages now uses Actions by default](https://github.blog/2022-08-10-github-pages-now-uses-actions-by-default/), theoretically any static web framework can be deployed using Actions, instead of the classic way: deploy from a branch. However, deploy from a branch is still available.

This project is a starter template for build and deploy Jekyll+Tailwindcss site on Github Pages, which can be deployed using Actions or deploy from a branch.

## Prerequisites

- You have created a Jekyll+Tailwindcss site
- The site is working fine locally
- Your environment is similar to the following
- You already have a Github account

## Environment

- Jekyll v4.3.2
- Tailwindcss v3.2.7
- Node.js v18.14
- ruby v3.1.2

*In the above version numbers `xxx.yyy.zzz`, if `xxx` is the same, generally there will not be any problem.*

## Publish to Github Pages

Just choose one of the delopyment methods below, and your site will be automatically build and deploy to Github Pages when you push to your `main` branch.

### Using Actions

Step 1: Copy [gh-pages-with-actions.yml](https://github.com/guox/jekyll-tailwind-starter/blob/main/.github/workflows/gh-pages-with-actions.yml) to your project `/.github/workflows/` directory.

Step 2: Set Github Pages Source to **Github Actions**

![Github Pages Source: Actions](/assets/images/ghpages-source-action.png)

### Deploy from a branch

Step 1: Copy [gh-pages-from-branch.yml](https://github.com/guox/jekyll-tailwind-starter/blob/main/.github/workflows/gh-pages-from-branch.yml) to your project `/.github/workflows/` directory.

Step 2: Set Github Pages Source to **Github Actions** and Branch to **gh-pages**

![Github Pages Source: from a branch](/assets/images/ghpages-source-branch.png)

*Note: You don't need to create **gh-page** branch in advance, when you push `gh-pages-from-branch.yml` to Github repo, **gh-pages** branch will be created automatically.*

## Source code and demo

See <https://github.com/guox/jekyll-tailwind-starter>

## License

MIT



