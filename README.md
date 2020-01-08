# First Steps with Hugo

Can we use Hugo to build a static site made of Jupyter notebooks?

To see this site, please [install Hugo](https://gohugo.io/getting-started/installing/), and then execute
```
git clone git@github.com:mwouts/first_steps_with_hugo.git
cd first_steps_with_hugo
hugo serve -D
```

## Part I - Hugo Markdown format

A page is either `_index.md` in a sub-directory of `content`, or any `.md` file in a sub-directory of content.

Hugo supports the inclusion of
- formatted text
- images (located in a folder with the same name as the page)
- figures (i.e. images with a custom size and caption), using the `figure` shortcode
- plotly graphs, using our custom `plotly` shortcode
- and probably soon, Jupyter Widgets, with two shortcodes: `widget-state`, and `widget`.
- can we support arbitrary Javascript output (Bokeh, itables...)?

If we can support all these output types, I'd be interested in implementing a Hugo Markdown format (with outputs) in Jupytext, and represent a notebook as a single `.md` file, with outputs in adjacent `.png`, `.json` or `.html` files.

## Part II - How to execute the notebooks

Some pages should be really short, e.g. chapter headings. Going further, can we split a notebook over many pages? To allow this we need to execute the pages (notebooks) sequencially, i.e. allow one notebook to depend on another one (i.e. load its variables, etc). A cache sytem would probably be required to make this usable.

