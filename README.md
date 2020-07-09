# jekyll-template
Simple template for creating openSUSE websites with jekyll

Please remember openSUSE is not SUSE, and neither this nor any other website with openSUSE branding is fit for webservers hosting on suse.com/suse.de domains or other SUSE related projects.

## General HOW-TO:

1. Use [Repository Generator](https://github.com/openSUSE/jekyll-template/generate) to create a new repositosiry based on this one
2. Edit the metadata in [_config.yml](https://github.com/openSUSE/jekyll-template/blob/master/_config.yml) to suit your project
3. Modify [index.md](https://github.com/openSUSE/jekyll-template/blob/master/index.md) to suit your site's needs, and add as many more .md and .html files as you need to expand the site

## How to build?

```bash
bundle install --path vendor/bundle
bundle exec jekyll build
```

Resulting site will be in `_site` directory.

## How to serve locally?

```bash
bundle install --path vendor/bundle
bundle exec jekyll serve
```

Visit <http://127.0.0.1:4000/> in your browser.
