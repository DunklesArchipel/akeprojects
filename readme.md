# AKE projects

My personal website summarizing my former and ongoing projects.

## Render the book locally

```sh
jupyter-book build docs
python -m http.server 8880 -b localhost --directory docs/_build/html &
```
