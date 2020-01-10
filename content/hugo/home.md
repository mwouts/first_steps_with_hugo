---
title: Home page & Site content
weight: 20
---

## The Home page

The home page is `_index.md` in the `content` folder.

## Creating a new section

The menu bar on the left reproduces the folder hierarchy in the `content` folder. So, if we want to have an entry named `Typing text` in that menu, we create a folder i.e. `text`, and there a `_index.md` file with the following header:

```
---
title: Typing text
weight: 100
---
```

(note that `weight` is used to determine the position relative to the other entries in the menu).

In that section/subfolder you can create more pages. Again, use `weight` to fix the order of your pages within a subfolder.