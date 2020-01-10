---
title: Installing Hugo
weight: 10
---

Hugo is super easy to install. I have followed the official [quick start](https://gohugo.io/getting-started/quick-start/), i.e.
- I installed Hugo
- then created this project with `hugo new site first_steps_with_Hugo`
- and downloaded the [Hugo Theme for technical documentation](https://github.com/thingsym/hugo-theme-techdoc) with
```powershell
cd first_steps_with_Hugo
git init
git submodule add https://github.com/thingsym/hugo-theme-techdoc themes/hugo-theme-techdoc
```
and then, I have edited `config.toml` and appended a line `theme = "hugo-theme-techdoc"`.

I have also changed the name of my site in the `config.toml` file, and converted the `toml` file to a YAML one as I am more used to YAML.

The site can be rendered locally at [http://localhost:1313/](http://localhost:1313/) with
```powershell
hugo serve -D
```
