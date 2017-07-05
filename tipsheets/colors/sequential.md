##Sequential
"Sequential data classes are logically arranged from high to low, and this stepped sequence of categories should be represented by sequential lightness steps. Terrain slope categories or population densities, for example, are well represented by sequental color schemes." - [ColorBrewer](https://web.natur.cuni.cz/~langhamr/lectures/vtfg1/mapinfo_2/barvy/colors.html)

### Sequential Sangria - Peach 

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $Sangria | ![\#9b0001](https://placehold.it/15/9b0001/000000?text=+) `#9b0001` | rgb(155,0,1) |
| $Tabasco | ![\#a72516](https://placehold.it/15/a72516/000000?text=+) `#a72516` | rgb(167,37,22) |
| $Poppy | ![\#b33c2a](https://placehold.it/15/b33c2a/000000?text=+) `#b33c2a` | rgb(179,60,42) |
| $Rust | ![\#bf523e](https://placehold.it/15/bf523e/000000?text=+) `#bf523e` | rgb(191,82,62) |
| $Salmon | ![\#cc6657](https://placehold.it/15/cc6657/000000?text=+) `#cc6657` | rgb(204,102,87) |
| $Coral | ![\#d77e6b](https://placehold.it/15/d77e6b/000000?text=+) `#d77e6b` | rgb(215,126,107) |
| $DustySalmon | ![\#e29684](https://placehold.it/15/e29684/000000?text=+) `#e29684` | rgb(187,168,143) |
| $DustyPink | ![\#edaf9e](https://placehold.it/15/edaf9e/000000?text=+) `#edaf9e` | rgb(226,150,132) |
| $SpringPeach | ![\#f6c9ba](https://placehold.it/15/f6c9ba/000000?text=+) `#f6c9ba` | rgb(246,201,186) |
| $Peach | ![\#ffe5d8](https://placehold.it/15/ffe5d8/000000?text=+) `#ffe5d8` | rgb(255,229,216) |

```
'#9b0001','#a72516','#b33c2a','#bf523e','#cc6657','#d77e6b','#e29684','#edaf9e','#f6c9ba','#ffe5d8'
```

```d3.scale.threshold()
.range(['#9b0001','#a72516','#b33c2a','#bf523e','#cc6657','#d77e6b','#e29684','#edaf9e','#f6c9ba','#ffe5d8']);
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
