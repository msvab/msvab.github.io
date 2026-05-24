# Michal Šváb

The source code for [svab.net](https://svab.net), built with [Jekyll](https://jekyllrb.com).

## Local setup

This repo is pinned to:

- Ruby `3.3.4` via [`.ruby-version`](/Users/michal-mbp/dev/msvab.github.io/.ruby-version:1)
- Bundler `2.5.5` via [Gemfile.lock](/Users/michal-mbp/dev/msvab.github.io/Gemfile.lock:310)
- GitHub Pages dependencies via [Gemfile](/Users/michal-mbp/dev/msvab.github.io/Gemfile:5)

The `github-pages` gem controls Jekyll and plugin compatibility. The Ruby version here is pinned for reproducible local builds with `rbenv`.
On recent macOS Command Line Tools installs, `./bin/setup` also patches the local `rbenv` Ruby if Ruby recorded `CXX=false`, which otherwise breaks native gems such as `eventmachine`.

### Install with rbenv

```bash
brew install rbenv ruby-build
rbenv init
```

Restart your shell, then from this repo:

```bash
rbenv install 3.3.4
./bin/setup
```

### Build

```bash
./bin/build
```

### Serve locally

```bash
./bin/serve
```

The local preview runs at `http://127.0.0.1:4000`.
