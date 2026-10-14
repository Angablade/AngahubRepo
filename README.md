# AngaHub Community Plugins

A repository for plugins and widgets made for AngaHub.

## Add this repository to AngaHub

1. Publish `catalog.json` at a stable, publicly accessible HTTPS URL.
2. Replace the example `sourceUrl` values in the catalog with the actual download URLs for your release ZIP files.
3. In AngaHub, open **Plugin Store** and add the URL to `catalog.json` as a plugin repository.

## Repository layout

- `catalog.json` — plugin repository catalog read by AngaHub.
- `packages/` — optional place to keep source/package ZIP files.
- `README.md` — repository information and publishing notes.

## Publishing a plugin

1. Package each plugin as a ZIP with a `manifest.json` at the package root and the files listed by that manifest.
2. Publish the ZIP as a release or at another stable HTTPS download URL.
3. Add an entry for it under the `plugins` array in `catalog.json`.
4. Include the plugin's ID, name, description, kind, category, version, source URL, and a short changelog.
5. Commit and publish the updated catalog.

For catalog structure and package fields, follow the AngaHub Plugin Developer Guide for the version of AngaHub you use.

## Notes

- Keep plugin IDs stable across releases.
- Only publish plugins you trust and have reviewed. Plugins may include JavaScript and Python code that runs within the AngaHub host.
