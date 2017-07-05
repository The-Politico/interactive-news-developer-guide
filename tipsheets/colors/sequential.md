##Sequential
"Sequential data classes are logically arranged from high to low, and this stepped sequence of categories should be represented by sequential lightness steps. Terrain slope categories or population densities, for example, are well represented by sequental color schemes." - [ColorBrewer](https://web.natur.cuni.cz/~langhamr/lectures/vtfg1/mapinfo_2/barvy/colors.html)

### Sequential Sangria - Peach 

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $Sangria | ![\#9b0001](https://placehold.it/15/9b0001/000000?text=+) `#9b0001` | rgb(155,0,1) |
| $Tabasco | ![\#af2311](https://placehold.it/15/af2311/000000?text=+) `#af2311` | rgb(175,35,17) |
| $Poppy | ![\#c33b22](https://placehold.it/15/c33b22/000000?text=+) `#c33b22` | rgb(195,59,34) |
| $Rust | ![\#d35234](https://placehold.it/15/d35234/000000?text=+) `#d35234` | rgb(211,82,52)|
| $Sockeye | ![\#d35234](https://placehold.it/15/d35234/000000?text=+) `#d35234` | rgb(211,82,52) |
| $Coral | ![\#e36849](https://placehold.it/15/e36849/000000?text=+) `#e36849` | rgb(227,104,73) |
| $DustySalmon | ![\#f08060](https://placehold.it/15/f08060/000000?text=+) `#f08060` | rgb(250,152,123) |
| $DustyPink | ![\#fa987b](https://placehold.it/15/fa987b/000000?text=+) `#fa987b` | rgb(250,152,123) |
| $SpringPeach | ![\#f6c9ba](https://placehold.it/15/f6c9ba/000000?text=+) `#f6c9ba` | rgb(246,201,186) |
| $Peach | ![\#ffe5d8](https://placehold.it/15/ffe5d8/000000?text=+) `#ffe5d8` | rgb(255,229,216) |

```
'#9b0001','#af2311','#c33b22','#d35234','#e36849','#f08060','#fa987b','#ffb297','#ffcbb7','#ffe5d8'
```

```d3.scale.threshold()
.range(['#9b0001','#af2311','#c33b22','#d35234','#e36849','#f08060','#fa987b','#ffb297','#ffcbb7','#ffe5d8']);
```

---

### Sequential Money - SeaFoam

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $Money | ![\#9b0001](https://placehold.it/15/46825a/000000?text=+) `#46825a` | rgb(70,130,90) |
| $Bills | ![\#578e69](https://placehold.it/15/578e69/000000?text=+) `#578e69` | rgb(87,142,105) |
| $SpringLeaves | ![\#699c79](https://placehold.it/15/699c79/000000?text=+) `#699c79` | rgb(105,156,121) |
| $NewMoss | ![\#79a887](https://placehold.it/15/79a887/000000?text=+) `#79a887` | rgb(118,165,132) |
| $BayLeaf | ![\#8bb597](https://placehold.it/15/8bb597/000000?text=+) `#8bb597` | rgb(139,181,151) |
| $Summer | ![\#9cc2a7](https://placehold.it/15/9cc2a7/000000?text=+) `#9cc2a7` | rgb(156,194,167) |
| $Oregano | ![\#aecfb8](https://placehold.it/15/aecfb8/000000?text=+) `#aecfb8` | rgb(174,207,184) |
| $Thyme| ![\#c0dcc9](https://placehold.it/15/c0dcc9/000000?text=+) `#c0dcc9` | rgb(192,220,201) |
| $DustySeafoam | ![\#d2e9da](https://placehold.it/15/d2e9da/000000?text=+) `#d2e9da` | rgb(210,233,218) |
| $Seafoam | ![\#e4f7eb](https://placehold.it/15/e4f7eb/000000?text=+) `#e4f7eb` | rgb(228,247,235) |

```
'#46825a','#578e69','#699c79','#79a887','#8bb597','#9cc2a7','#aecfb8','#c0dcc9','#d2e9da','#e4f7eb'

```

```
d3.scale.threshold()    .range(['#46825a','#578e69','#699c79','#79a887','#8bb597','#9cc2a7','#aecfb8','#c0dcc9','#d2e9da','#e4f7eb']);
```

---
