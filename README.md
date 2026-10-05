# OOPSLA 2026 slides

Talk slides and a poster, served by GitHub Pages at
<https://sweetsinpackets.github.io/oopsla26-slides/>.

- **When Lifetimes Liberate: A Type System for Arenas with Higher-Order
  Reachability Tracking** (OOPSLA 2026): slides in `arena/`, poster in
  `poster/poster.pdf`, [paper](https://doi.org/10.1145/3798254).
- **Reachability Types: Tracking Resources in Higher-Order Programs**
  (iWACO 2026, invited talk): slides in `reachability/`.

## Viewing locally

The decks load their slides over HTTP, so opening an `index.html` as a file
does not work. Serve the repository and open a deck:

```
python3 -m http.server 8000     # then open http://localhost:8000/arena/
```

Add `?view=scroll` to a deck's URL for one long scrollable page.

MathJax, Mermaid and Chart.js load from a CDN. To run a deck without a
network, run `npm install` in its directory and point the `localPaths`
entries at the top of its `index.html` to `./node_modules/...`.

## Built with

[Reveal.js](https://revealjs.com/),
[MathJax 4](https://docs.mathjax.org/en/v4.1/),
[Mermaid](https://mermaid.js.org/),
[Chart.js](https://www.chartjs.org/),
[highlight.js](https://highlightjs.org/), and the
[Cascadia Code](https://github.com/microsoft/cascadia-code) font (SIL OFL,
license in each deck's `dist/custom/fonts/`).
