source "https://rubygems.org"

# ---------------------------------------------------------------------------
#  LOCAL PREVIEW TOOLCHAIN
#
#  Uses plain Jekyll 4, which supports modern Ruby (including Ruby 4.0) out of
#  the box — unlike the `github-pages` gem, which pins the very old Jekyll 3.9
#  and breaks on new Ruby versions.
#
#  This file affects ONLY your local `jekyll serve` preview. Your live site is
#  still built by GitHub Pages using its own toolchain, so deployment is
#  unchanged.
#
#  Run with:  bundle exec jekyll serve --livereload
# ---------------------------------------------------------------------------

gem "jekyll", "~> 4.3"

# Force the Dart-Sass converter: it ships as a precompiled binary, so no C
# compiler is needed (the older sassc-based 2.x line fails to build on Windows).
gem "jekyll-sass-converter", "~> 3.0"

# Site plugins (must match the `plugins:` list in _config.yml).
group :jekyll_plugins do
  gem "jekyll-paginate"
  gem "jekyll-sitemap"
  gem "jekyll-gist"
  gem "jekyll-feed"
  gem "jekyll-redirect-from"
end

# Standard-library gems that Ruby 3.4+/4.0 removed from the defaults but that
# Jekyll still needs at runtime. `webrick` powers `jekyll serve` on Ruby 3+.
gem "webrick"
gem "csv"
gem "base64"
gem "bigdecimal"
gem "logger"

# Windows has no system timezone database, so Jekyll needs these to resolve the
# site's timezone. (Pure-Ruby gems — safe on any platform.)
gem "tzinfo"
gem "tzinfo-data"
