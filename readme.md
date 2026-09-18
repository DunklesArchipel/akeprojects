# AKE projects

My personal website summarizing my former and ongoing projects.

## Developer instructions

Install [pixi](https://pixi.sh), then install dependencies

```sh
pixi install
```

Render the book locally as static HTML

```sh
pixi run build-html
```

Explore the page by either opening the `index.html` in `docs/_build/html` or by
starting the development server (with live reload) on <http://localhost:3000>

```sh
pixi run start
```

To clean the build output:

```sh
pixi run clean
```
