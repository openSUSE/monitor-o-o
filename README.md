# openSUSE Monitor
The home page for the openSUSE Infrastructure

## How to build?

```sudo zypper in awk gcc-c++ git-core make openssl-devel 'rubygem(bundler)' 'rubygem(jekyll)' 'rubygem(strscan)' ruby-devel

Unfortunately not all of these packages are available in the distribution repositories.

After having satisfied the dependencies, it should be enough to call:
```bash
bundle install
```
followed by a:
```bash
bundle exec jekyll build
```

Our .bundle/config already contains the path for the vendor files.
If you need to change this (for whatever reason), you can overwrite 
this path via: 
```bash
bundle config set path 'vendor/bundle'
```
but we recommend not to do this. 

Older systems might require to define the installation path for the 
additional vendor files via command line option. In this case, just
enhance the initial install call: 
```bash
bundle install --path vendor/bundle
```

Resulting site will be in `_site` directory.

## How to serve locally?

```bash
bundle install --path vendor/bundle
bundle exec jekyll serve
```

Visit <http://127.0.0.1:4000/> in your browser.
