---
title: Interactive tables
---

If I include directly the outputs from https://mwouts.github.io/itables/ here, I get this error:
_ReferenceError: require is not defined_

So we are missing the `require.js` library.

https://discourse.gohugo.io/t/best-way-to-include-javascript-libraries-in-hugo-sites/13614

```
{{</* include file="content/tables/dt.html" */>}}
```

{{< include file="content/tables/dt.html" >}}
