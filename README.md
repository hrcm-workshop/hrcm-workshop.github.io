# HRCM Workshop Webpages (hrcm-workshop.github.io)

## Previewing your changes

Generally speaking, follow the instructions at

https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll#building-your-site-locally

to build the website locally, and run a webserver to inspect your local changes.

Run the following to re-build automatically when your files change:
```
bundle exec jekyll serve --host 0.0.0.0 --incremental
```

## Creating a page for a new year
To duplicate a page from the previous year (let's say 2021), to create a page for the new year (let's say 2022), the following changes are necessary:

1. Copy the static files with `cp -r 2021/ 2022/`
2. Copy the layout file with `cp _layouts/layout_2021.html _layouts/layout_2022.html`
3. Make copies of `_includes/head_2021.html`, `_includes/header_2021.html`, and `_includes/footer_2021.html`
4. Add entry button for new year in `_includes/header_common.html`
5. Copy the main content file with `cp _pages/home_2021.md _pages/home_2022.md`
6. Edit the top lines in `_pages/home_2022.md` such that the new year is reflected, the new files are used, and the new page is actually generated by Jekyll.
7. Edit `index.html` to refresh to the new page.

## Acknowledgements

Website based on those of the [A3DE](https://github.com/a3de-hri/a3de-hri.github.io) and [Gaze](https://github.com/gazeworkshop/gazeworkshop.github.io) workshops.
