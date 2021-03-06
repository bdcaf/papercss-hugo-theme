# PaperCSS

A Hugo theme made with PaperCSS, the less formal CSS framework.

A fork of [papercss-hugo-theme](https://github.com/zwbetz-gh/papercss-hugo-theme).
This fork was built as companion to [r-hugo-papercss-template](https://github.com/bdcaf/r-hugo-papercss-template).

This branch contains the scss files from [papercss](https://github.com/papercss/papercss) version 1.6.1.

## new dependencies

This theme uses hugos SASS and postcss capabilities.  
However it needs [node](https://nodejs.org/en/) to be installed to setup required node modules in the project. 
Copy the file 'node_modules/' into the site directory (not the theme directory!).
Run `npm install ci` in the site folder to set it up.


## Table of contents

- [Demo](#demo)
- [Minimum Hugo version](#minimum-hugo-version)
- [Installation](#installation)
- [Updating](#updating)
- [Run example site](#run-example-site)
- [Configuration](#configuration)
- [Favicons](#favicons)
- [Shortcodes](#shortcodes)
- [Disable toc for a blog post](#disable-toc-for-a-blog-post)
- [Disable summary for a blog post](#disable-summary-for-a-blog-post)
- [Getting help](#getting-help)
- [Credits](#credits)

## Demo

https://bdcaf.github.io/papercss-hugo-theme/

## Minimum Hugo version

Hugo version `0.54.0` or higher is required. View the [Hugo releases](https://github.com/gohugoio/hugo/releases) and download the binary for your OS.

## Installation

From the root of your site:

```
git submodule add https://github.com/zwbetz-gh/papercss-hugo-theme.git themes/papercss-hugo-theme
```

## Updating

From the root of your site:

```
git submodule update --remote --merge
```

## Run example site

From the root of `themes/papercss-hugo-theme/exampleSite`:

```
hugo server --themesDir ../..
```

## Configuration

Copy the `config.toml` or `config.yaml` from the [`exampleSite`](https://github.com/zwbetz-gh/papercss-hugo-theme/tree/master/exampleSite), then edit as desired. 

## Favicons

Upload your image to [RealFaviconGenerator](https://realfavicongenerator.net/) then copy-paste the generated favicon files under `static`. 

## Shortcodes

For page bundles to link to included files.

 - bundle-file `{{< bundle-file name="test.r" caption="description" >}}`
 - bundle-image `{{< bundle-image name="picture.jpg" caption="description" >}}`

See the [full list of supported shortcodes of the parent theme](https://papercss-hugo-theme.netlify.com/papercss-shortcodes/).

## Disable toc for a blog post

Blog posts that have two or more subheadings (`<h2>`s) automatically get a table of contents. To disable this set `toc` to `false`. For example:

```
---
title: "My page with a few headings"
toc: false
---
```

## Disable summary for a blog post

The homepage blog post listing shows a summary for each post. To disable this for an individual post set `summary` to `false`. For example:

```
---
title: "My page with some stellar content"
summary: false
---
```

## Getting help

If you run into an issue that isn't answered by this documentation or the [`exampleSite`](https://github.com/zwbetz-gh/papercss-hugo-theme/tree/master/exampleSite), then visit the [Hugo forum](https://discourse.gohugo.io/). The folks there are helpful and friendly. **Before** asking your question, be sure to read the [requesting help guidelines](https://discourse.gohugo.io/t/requesting-help/9132). Feel free to tag me in your question, my forum username is [@zwbetz](https://discourse.gohugo.io/u/zwbetz/summary).

## Credits

Thank you to [Rhyne Vlaservich](https://www.vlaservich.com/) for creating [PaperCSS](https://www.getpapercss.com/), and all the  [contributors](https://github.com/papercss/papercss/graphs/contributors).
