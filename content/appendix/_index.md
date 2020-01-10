---
title: Appendix
linkTitle: 
weight: 500
---

## Installing Hugo

I have followed the official [quick start](https://gohugo.io/getting-started/quick-start/), i.e.

- installed Hugo
- Created this project with `hugo new site first_steps_with_Hugo`
- Downloaded the [Learn theme](https://learn.netlify.com) with
```powershell
cd first_steps_with_Hugo
git init
git submodule add https://github.com/matcornic/hugo-theme-learn.git themes/learn
```
and then, I have edited `config.toml` and appended a line `theme = "learn"`.

I have also changed the name of my site in the `config.toml` file, and converted the `toml` file to a YAML one as I am more used to YAML.

At this stage, we run 
```powershell
hugo serve -D
```
and get an empty web site at [http://localhost:1313/](http://localhost:1313/).

## Creating the index

Now I create an empty file `_index.md` in the `content` folder. The content of the file is displayed below the site title.

## Creating a new chapter

The menu bar on the left reproduces the folder hierarchy in the `content` folder. So, if we want to have an entry named `Typing text` in that menu, we create a folder i.e. `text`, and there a `_index.md` file with the following header:

```
---
title: Typing text
weight: 100
---
```

(note that `weight` is used to determine the position relative to the other entries in the menu).

# Alternative themes

The `learn` theme is great, but I was not able to embed HTML content that uses `requirejs` (e.g. Jupyter widgets or interactive tables).

The `ananke` theme has no such issue, but I was missing the navigation menu.

The `hugo-book` theme looks great, but there I don't see how to go to the next chapter.

The `hugo-theme-techdoc` works super well! It even has the _edit on GitHub_ link. The only issue I saw was that the first interactive table was breaking the lateral menu. 

The `docsy` theme has more requirements than the other ones: I had to uninstall `hugo` and instead install `hugo-extended`, install `nodejs` (all that using `choco (un)install` as an administrator), and then restarted powershell, cd to my project, and ran `npm install -D --save autoprefixer` and `npm install -D --save postcss-cli`... and finally got a few additional errors.
