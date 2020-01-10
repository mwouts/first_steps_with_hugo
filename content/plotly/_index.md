---
title: Plotly graphs in Hugo
weight: 30
---

We can embed interactive Plotly graphs[^1] using a [`plotly` shortcode](https://github.com/mwouts/first_steps_with_hugo/blob/master/layouts/shortcodes/plotly.html), which owes much to Igor Gotlibovych's [example](https://ig248.gitlab.io/post/2018-11-05-plotly-sample/).

[^1]: The plot here was created using [easyplotly](https://github.com/mwouts/easyplotly), using data from the [World Bank](https://data.worldbank.org/).

```
{{</* plotly json="world_population.json" */>}}
```

{{< plotly json="world_population.json" >}}
