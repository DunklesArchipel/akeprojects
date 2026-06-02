# Project Guidelines

This is a [MyST](https://mystmd.org/) documentation site for a AKEs projects webpage.

## Editing Conventions

- **HTML comments** (`<!-- ... -->`) embedded in Markdown files are instructions to the agent — treat them as tasks to perform on the surrounding content, unless explicitly stated otherwise.
- **Always fix typos** immediately whenever you encounter them, without waiting to be asked.

## Figures

Use the MyST `{figure}` directive. Single-image example:

```markdown
```{figure} files/figures/research/my_image.png
:height: 200px
:label: fig-my-label

Caption text.{cite}`author_title_year`
```
```

Multi-image (grid) example:

```markdown
```{figure}
:label: fig-my-label
:class: grid grid-cols-2

![Alt text left](files/figures/research/left.png)

![Alt text right](files/figures/research/right.png)

Left caption (left) and right caption (right).{cite}`author_title_year`
```
```

## Chemical Formulas

Use KaTeX with the `\ce{}` command (mhchem):

- Inline: `$\ce{NiOOH}$`, `$\ce{H2O2}$`, `$\ce{NiO2}$`
- Block equations use standard KaTeX `$$...$$`

## Citations

Citations use the MyST `{cite}` role: `{cite}`author_title_year`` (comma-separated for multiple).
Place citations **directly after** the period with no space: `text.{cite}`key`` — never before it.
References are defined in `docs/references.bib`.

## Build & Tooling

[pixi](https://pixi.sh) is the development environment manager. Tasks and dependencies are defined in `pixi.toml`. Use `pixi run <task>` to execute project tasks.

- `pixi run start` — start the MyST development server
- `pixi run build` — build the site
- `pixi run clean` — clean build artifacts
- `pixi run check-links` — check all external links

See [/memories/repo/tooling.md] for notes on the local environment.
`rg` is not available; use `grep -RInE` for text search.

## Project Structure

- `docs/` — MyST source files
- `docs/files/figures/` — figure assets, organized by page (e.g. `research/`)
- `docs/styles/extra.css` — custom CSS
- `docs/references.bib` — BibTeX bibliography
- `pixi.toml` — environment and task definitions
