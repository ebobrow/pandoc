```
% pandoc -t markdown-citations
---
csl: command/oscola.csl
references:
- DOI: 10.1086/504343
  author:
  - family: Olson
    given: Hope A.
  container-title: Library Quarterly
  id: item1
  issue: 1
  issued:
    date-parts:
    - - 2006
  page: '19-35'
  title: 'Codes, costs, and critiques: The organization of information
    in *Library Quarterly*, 1931--2004'
  title-short: 'Codes, costs, and critiques'
  type: 'article-magazine'
  volume: 76
- id: item2
  title: Second title
---

Foo [@item1]. Bar [@item2]. Baz [@item1].
^D
Foo.[^1] Bar.[^2] Baz.[^3]

::: {#refs .references}
::: {#ref-item1}
Olson HA, 'Codes, Costs, and Critiques: The Organization of Information
in *Library Quarterly*, 1931--2004' (2006) 76 *Library Quarterly* 19
:::

::: {#ref-item2}
'Second Title'
:::
:::

[^1]: Hope A Olson, 'Codes, Costs, and Critiques: The Organization of
    Information in *Library Quarterly*, 1931--2004' (2006) 76 *Library
    Quarterly* 19.

[^2]: 'Second Title'.

[^3]: Olson (n 1).
```