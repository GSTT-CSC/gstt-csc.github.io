#after any changes to the Gemfile, execute bundle update!

source "https://rubygems.org"

ruby ">= 3.1.0"


group :jekyll_plugins do
    gem "jekyll", "~> 4.2"      # Core Jekyll dependency – version compatible with Ruby 3.4+

    # Search engine optimization plugins
    gem "jekyll-seo-tag"        # Automatically adds useful <meta> tags in <head>
    gem "jekyll-sitemap"        # Generates sitemap.xml for search engine indexing
    gem "jekyll-feed"           # Generates an RSS feed (feed.xml) for blog/news content
    gem "jekyll-redirect-from"  # Allows setting up clean redirects


    # Development plugins
    gem "jekyll-watch"          # Watches file changes and rebuilds the site automatically
    gem "webrick"               # Required to serve Jekyll sites locally (for Ruby >= 3.0)
  end
  
# Delete the following lines if not on Windows: 
# Performance-booster for watching directories on Windows
gem "wdm", ">= 0.1.0" if Gem.win_platform?

