# RapidMiner Documentation Site

A simple documentation system to provide RapidMiner documentation at [docs.rapidminer.com](http://docs.rapidminer.com). This setup is built using [Jekyll](http://jekyllrb.com/), a plain text CMS for static websites. 

## Inspiration

* [KISSmetrics](http://support.kissmetrics.com/) -- Awesome layout and structure, this is built with Jekyll and is hosted at Github, allowing anyone to fork and contribute to the documentation.
* [memsql](http://developers.memsql.com/docs/latest/#) -- Nice design

## Install & Run

Jekyll is a command line Ruby tool, so you'll need to have Ruby on Rails configured on your machine in order to use the `gem` package manager. [Instructions for that can be found here](https://gorails.com/setup/osx/10.10-yosemite).

1. Install Jekyll on your system if you don't already have it: `gem install jekyll` or `sudo gem install jekyll`
1. Clone *docs.rapidminer.com* to your system: `got clone https://kleary@gitlab.rapid-i.com/stash/scm/web/docs.rapidminer.com.git ~/Sites/docs.rapidminer.com`
1. Browse to the repo folder: `cd ~/Sites/docs.rapidminer.com`
1. Start the server: `jekyll serve`

That's it! Your site is now available locally on your machine at [http://0.0.0.0:4000/](http://0.0.0.0:4000/)

## Publish *(proposed)*

Jekyll can be deployed to GitHub and served using GitHub pages for free. Here's how to do it:

1. Add a remote for GitHub: `git add remote github git@github.com:rapidminer-docs/rapidminer-docs.git`
1. Push your changes to the new remote: `git push github master`
1. 

## Directory Structure

This is a half complete template that uses the following directory structure for organization:

* **_data** -- Used for data feeds, this stores the data file for constructing the left hand tree menu
* **_includes** -- Shared templates for footer, header and navigation area
* **_layouts** -- Full page layouts, currently there's only one needed
* **_plugins** -- Plugins to extend the system and provide dynamic functionality, currently there's a plugin configured for serving Markdown (.md) content models
* **_site** -- The compiled build location where the site is served from, don't put anything in here

