# Dapla Landscape (landscape2)

This repository is scaffolded to run [`landscape2`](https://github.com/cncf/landscape2).

## Files

- `data.yml`: categories, subcategories, and landscape items
- `settings.yml`: required global settings for build output
- `guide.yml`: category guide content shown in the generated site
- `logos/`: SVG logos referenced by `data.yml`

## Build

```bash
LANDSCAPE2=/Users/johnksv/code/ssb/temp/landscape2/target/debug/landscape2

$LANDSCAPE2 build \
  --data-file ./data.yml \
  --settings-file ./settings.yml \
  --guide-file ./guide.yml \
  --logos-path ./logos \
  --output-dir ./build
```

## Serve locally

```bash
LANDSCAPE2=/Users/johnksv/code/ssb/temp/landscape2/target/debug/landscape2

$LANDSCAPE2 serve --landscape-dir ./build
```
