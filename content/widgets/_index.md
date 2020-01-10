---
title: Jupyter widgets in Hugo
weight: 40
---

## Loading the widgets

We first need to load the widget state with our [`widget_state` shortcode](https://github.com/mwouts/first_steps_with_hugo/blob/master/layouts/shortcodes/widget-state.html)
```
{{</* widget-state state="/content/widgets/widget_state.json" */>}}
```

{{< widget-state state="/content/widgets/widget_state.json" >}}

## Displaying the widgets

Now we can display the widgets that were originally in a Jupyter notebook with our [`widget` shortcode](https://github.com/mwouts/first_steps_with_hugo/blob/master/layouts/shortcodes/widget.html):

```
{{</* widget model_id="6593b7fef9874465b5f323790e13d6ba" */>}}
```

{{< widget model_id="6593b7fef9874465b5f323790e13d6ba" >}}

```
{{</* widget model_id="6593b7fef9874465b5f323790e13d6ba" */>}}
{{</* widget model_id="ab00a002a80a420c85b6a9a72e569e2d" */>}}
```

{{< widget model_id="6593b7fef9874465b5f323790e13d6ba" >}}
{{< widget model_id="ab00a002a80a420c85b6a9a72e569e2d" >}}

Above we're seeing an integer slider, and then, the same integer slider repeated, together with a float slider. The two sliders were linked in the notebook, and the link remains active here.