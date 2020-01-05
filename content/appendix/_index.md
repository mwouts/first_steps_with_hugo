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
weight: 5
---
```

(note that `weight` is used to determine the position relative to the other entries in the menu).

