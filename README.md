# Secret Rhythm Project band website

HEY: Make sure not to commit files > 50MB. They get rejected from Github and it's a huge pain in the ass.


Jekyll static site with [Alembic](https://alembic.darn.es/#as-a-jekyll-theme) theme hosted on [Netflify](https://netflify.com) as [secretrhythm.com](https://secretrhythm.com).

## Setup

Install ruby, gem, bundler. Arch cmds:

* yay rbenv
* yay ruby-build
* rbenv install 2.6.10
* rbenv init (add eval "$(rbenv init - bash)" to the end of .bash_profile and restart shell)
* rbenv local 2.6.10 (run this in the project folder)
* gem install bundler:2.2.25

Then:

	bundler install

On Debian, nokogiri requires `sudo gem install nokogiri --platform=x86_64-linux`.

To run:

	bundler exec jekyll serve

To build:

    bundler exec jekyll build

Automatic deployment to netlify on push to master.

