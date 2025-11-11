# spatial-cluster-analysis

## Cluster Analysis — Decision Tree

This folder contains the Graphviz decision tree used in the project. The notebook `decision_graph.ipynb` renders the diagram and saves two outputs in this folder:

- `spatial_analysis_decision_tree_highres.png` — high-resolution PNG (raster)
- `spatial_analysis_decision_tree.svg` — vector SVG (scales cleanly)

How to include the SVG in Markdown (works on GitHub Pages and in repository README):

Markdown image:

```markdown
![Decision tree](spatial_analysis_decision_tree.svg)
```

Or use an HTML img tag to control size:

```html
<img src="spatial_analysis_decision_tree.svg" alt="Decision tree" width="1200" />
```

Notes
- SVG is preferred for crisp diagrams and for embedding into GitHub Pages. If you need raster PNG at a specific pixel size, convert the SVG to PNG with a tool like `rsvg-convert`, `inkscape` or `CairoSVG`.
- The notebook writes the SVG directly using Graphviz (`format='svg'`). If you want interactive or scripted SVG, place the SVG on a GitHub Pages HTML page (raw HTML), as GitHub's README sanitizer may remove embedded scripts in repo Markdown.
