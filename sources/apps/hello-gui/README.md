# Hello GUI

Minimal GUI app for the LUR workflow.

This directory is a standard LazyCat LPK project:

- `package.yml` contains application metadata and permissions.
- `lzc-manifest.yml` contains runtime services and routes.
- `lzc-build.yml` contains the official LPK build entry.
- `recipe.yml` contains LUR repository metadata.

The included `docker-compose.yml` is only retained as compatibility input and
reference. CI should build the installable `.lpk` from the official LPK project
files and publish the signed result through `dist/`.
