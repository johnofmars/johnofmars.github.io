# Welcome to Jekyll!
#
# This config file is meant for settings that affect your whole blog, values
# which you are expected to set up once and rarely edit after that. If you find
# yourself editing this file very often, consider using Jekyll's data files
# feature for the data you need to update frequently.
#
# For technical reasons, this file is *NOT* reloaded automatically when you use
# 'bundle exec jekyll serve'. If you change this file, please restart the server process.

# Site settings
# These are used to personalize your new site. If you look in the HTML files,
# you will see them accessed via {{ site.title }}, {{ site.email }}, and so on.
# You can create any custom variable you would like, and they will be accessible
# in the templates via {{ site.myvariable }}.
title: Fighting Lion Club
masthead_title: "Lion Club"
logo: "/assets/images/88x88.png"
email:
description: >- # this means to ignore newlines until "baseurl:"
  A community guide to Destiny 2’s Exotic Energy Grenade Launcher
twitter_username: johnofmars
github_username: johnofmars
minimal_mistakes_skin: dark
search: true
search_full_content      : true

teaser: /assets/images/teaser.jpg

# Build settings
markdown: kramdown
remote_theme: mmistakes/minimal-mistakes
# Outputting
permalink: /:categories/:title/
paginate: 1 # amount of posts to show
paginate_path: /page:num/
timezone: # https://en.wikipedia.org/wiki/List_of_tz_database_time_zones

include:
  - _pages
  - _posts
  - _docs

# Exclude from processing.
# The following items will not be processed, by default. Create a custom list
# to override the default setting.
# exclude:
#   - Gemfile
#   - Gemfile.lock
#   - node_modules
#   - vendor/bundle/
#   - vendor/cache/
#   - vendor/gems/
#   - vendor/ruby/

# Plugins (previously gems:)
plugins:
  - jekyll-paginate
  - jekyll-sitemap
  - jekyll-gist
  - jekyll-feed
  - jemoji
  - jekyll-include-cache

author:
  name   : "Fighting Lion"
  avatar : "/assets/images/bio-photo.png"
  bio    : "An Exotic Grenade Launcher in Destiny 2"

footer:
  links:
    - label: "Twitter"
      icon: "fab fa-fw fa-twitter-square"
      url: "https://twitter.com/johnofmars"

defaults:
  # _docs
  - scope:
      path: ""
      type: docs
    values:
      layout: single
      author_profile: false
      read_time: false
      comments: false
      share: true
      related: true
      sidebar:
        title: "Fighting Lion"
        image: /assets/images/sidebar_photo.png
        image_alt: "Fighting Lion"
        text: "An Exotic Grenade Launcher in Destiny 2."
        nav: "docs"
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: false
      read_time: false
      comments: false
      share: true
      related: true
      sidebar:
        title: "Fighting Lion"
        image: /assets/images/sidebar_photo.png
        image_alt: "Fighting Lion"
        text: "An Exotic Grenade Launcher in Destiny 2."
        nav: "docs"
  # _pages
  - scope:
      path: "_pages"
      type: pages
    values:
      layout: single
      author_profile: false
      sidebar:
        title: "Fighting Lion"
        image: /assets/images/sidebar_photo.png
        image_alt: "Fighting Lion"
        text: "An Exotic Grenade Launcher in Destiny 2."
        nav: "docs"

category_archive:
  type: liquid
  path: /categories/
tag_archive:
  type: liquid
  path: /tags/