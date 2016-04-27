## Documentation for TerriaJS

This repository contains:

- tools for building a documentation site from TerriaJS (in the `master` branch)
- the resulting Github Pages site (in the `gh-pages` branch)

### Installation

```
git clone https://github.com/TerriaJS/Documentation
cd Documentation
git clone --branch gh-pages https://github.com/TerriaJS/Documentation site

# Install mkdocs. Preferably you'd do this with a virtualenv.
pip install mkdocs 
```

### Updating

Assuming your local TerriaJS is up to date and available at ../../terriajs:

```
bash rebuild.sh

pushd site
git add --all . && git commit -m Update && git push
popd 
```