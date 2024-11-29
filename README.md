# willlumm.github.io

My personal website.

## Development

### Install Jekyll
https://jekyllrb.com/docs/installation/windows/
1. Download `Ruby+Devkit` from https://rubyinstaller.org/downloads/ and install.
1. Run `ridk install` on last step of installation and select `MSYS2 and MINGW development toolchain`.
1. Run `gem install jekyll bundler`.

### Build Site Locally
https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll
1. Run `bundle install`.
1. Run `bundle exec jekyll serve`.

When your theme is released, only the files in `_layouts`, `_includes`, and `_sass` tracked with Git will be released.