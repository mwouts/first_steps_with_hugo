---
title: HTML table in the Markdown file
---

In this document the table is directly embedded in the Markdown file

## A simple markdown table

Works well

| First column | Second column |
| -----------: | ------------: |
|            1 |             2 |


## A simple HTML table

Including HTML code directly in the Markdown file does not seem to work. Do we need to call `safeHTML`?

<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>