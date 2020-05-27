# Parcel Dist Cleaner

### A script that removes all files from the dist directory.

Useful when using Parcel Bundler before using the `parcel build` command, as files are bundled in the dist directory with unique serial numbers and are not overwritten.

`npm i parcel-dist-cleaner`

Node useage:

`node ./node_modules/parcel-dist-cleaner/distCleaner`

NPM script useage with Parcel: (package.json)

```json
...
  "scripts": {
    "start": "parcel src/index.html --open",
    "clean": "node ./node_modules/parcel-dist-cleaner/distCleaner",
    "prod": "npm run clean && parcel build src/index.html"
  },
...

```
