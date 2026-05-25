# LazyPort LUR

This repository is a minimal LUR source repository for LazyCat applications.

User-installable `.lpk` packages are not stored here by hand. The `sources/`
directory contains standard LazyCat LPK projects; CI should build signed `.lpk`
files with the official `lzc-cli` flow and publish them under `dist/`.

## Layout

```text
sources/
  repo.yml
  profiles/default.yml
  apps/hello-gui/
    package.yml
    lzc-manifest.yml
    lzc-build.yml
    recipe.yml
    docker-compose.yml
    README.md
```

## Example App

`sources/apps/hello-gui` defines a tiny web GUI as a standard LPK project. The
included `docker-compose.yml` is retained as compatibility input/reference; the
official build inputs are `package.yml`, `lzc-manifest.yml`, and
`lzc-build.yml`.
