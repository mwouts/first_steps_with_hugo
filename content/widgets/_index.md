---
title: Jupyter widgets in Hugo
weight: 40
---

To begin with, we load the widget state with
```
{{</* widget-state state="/content/widgets/widget_state.json" */>}}
```

{{< widget-state state="/content/widgets/widget_state.json" >}}

We first display an IntSlider:

```
{{</* widget model_id="6593b7fef9874465b5f323790e13d6ba" */>}}
```

{{< widget model_id="6593b7fef9874465b5f323790e13d6ba" >}}

Then we show the same int slider, together with a float slider that is linked to the first one:

```
{{</* widget model_id="6593b7fef9874465b5f323790e13d6ba" */>}}
{{</* widget model_id="ab00a002a80a420c85b6a9a72e569e2d" */>}}
```

{{< widget model_id="6593b7fef9874465b5f323790e13d6ba" >}}
{{< widget model_id="ab00a002a80a420c85b6a9a72e569e2d" >}}
