---
title: Interactive tables
---

If I include directly the outputs from https://mwouts.github.io/itables/ here, I get this error:
_ReferenceError: require is not defined_

There are two ways to remove the dependency on the `require.js` library:
1. Replace the calls to `require` with a script with `type="module"` that does `import * as datatables from "https://cdn.datatables.net/1.10.19/js/jquery.dataTables.min.js";`
2. Load `jQuery` and `datatables` with no call to `require`, just like in the [zero configuration example for datatables.net](https://datatables.net/examples/basic_init/zero_configuration.html)

See also: https://discourse.gohugo.io/t/best-way-to-include-javascript-libraries-in-hugo-sites/13614

## Table from a notebook

```
{{</* include file="content/tables/dt.html" */>}}
```

{{< include file="content/tables/dt.html" >}}

## Table from the zero-configuration example

```
{{</* include file="content/tables/dt2.html" */>}}
```

{{< include file="content/tables/dt2.html" >}}

