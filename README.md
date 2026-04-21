# Dapla Landscape (landscape2)

This repository is scaffolded to run [`landscape2`](https://github.com/cncf/landscape2).

## Files

- `data.yml`: categories, subcategories, and landscape items
- `settings.yml`: global settings for build output
- `guide.yml`: category guide content shown in the generated site
- `logos/`: logos referenced by `data.yml`

## Contributing

```shell
brew install cncf/landscape2/landscape2
```

### Build

```shell
landscape2 build \
  --data-file ./data.yml \
  --settings-file ./settings.yml \
  --guide-file ./guide.yml \
  --logos-path ./logos \
  --output-dir ./build
```

### Serve locally

```shell
landscape2 serve --landscape-dir ./build
```

Site is avaiable on `<localhost>/dapla-landscape`.
The reason for the base path is that we host the webpage on github pages.
