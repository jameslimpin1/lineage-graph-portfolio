# James's lineage graph

A single-page, dbt-docs-styled portfolio site — the whole thing is a hand-sketched
lineage graph (DAG) of James Limpin's career, skills, and projects.

## Run locally

```
python3 -m http.server 8000
```

Then open http://localhost:8000

## Edit content

All portfolio content lives in the `const models = [...]` array near the top of
the `<script>` tag in `index.html`. Each entry has `id`, `layer`, `name`,
`description`, `columns`, `sql`, `tags`, `depends_on`, and `links`. Edit that
array to update skills, roles, projects, or links — the graph, side panel, and
selector bar all read from it.

## Deploy to GitHub Pages

1. Create a GitHub repo and push this folder to it.
2. In the repo settings, go to **Pages** → set source to the `main` branch, root folder.
3. The site will be live at `https://<username>.github.io/<repo>/`.
