# Sass Project

A small responsive listing-page layout built with HTML and Sass. The page contains
three sample content items, each with a category, heading, summary, and a
placeholder media area.

## Project files

- `home.html` — the page markup.
- `style.scss` — Sass source, including color, spacing, and breakpoint variables
  plus mixins for reusable layout and typography.
- `style.css` — compiled stylesheet loaded by `home.html`.
- `style.css.map` — source map generated during Sass compilation.
- `.vscode/mcp.json` — VS Code MCP server configuration. It currently lists the
  GitHub MCP endpoint; it does not define a Sass MCP server.

## Sass development

Install the Dart Sass command-line tool if it is not already installed:

```sh
npm install --global sass
```

From the project root, start Sass in watch mode. It recompiles `style.scss` to
`style.css` whenever the source changes:

```sh
sass --watch style.scss:style.css
```

Keep this command running while editing Sass. The page uses the generated
`style.css`, so compile the Sass before previewing changes.

## Preview the page

In a second terminal, start a local static web server from the project root:

```sh
python3 -m http.server 8000
```

Open <http://localhost:8000/home.html> in a browser. Stop either running command
with `Ctrl+C`.
