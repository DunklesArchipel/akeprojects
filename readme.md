# AKE projects

My personal website summarizing my former and ongoing projects.

## Developer instructions

Install dependencies

```sh
mamba env create --file environment.yaml
mamba activate akeprojects
```

Render the book locally

```sh
jupyter-book build docs
```

Explore the page by either opening the `index.html` in `docs/_build/html` or use

```sh
python -m http.server 8880 -b localhost --directory docs/_build/html &
```
