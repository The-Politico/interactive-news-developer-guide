##Sequential
"Sequential data classes are logically arranged from high to low, and this stepped sequence of categories should be represented by sequential lightness steps. Terrain slope categories or population densities, for example, are well represented by sequental color schemes." - [ColorBrewer](https://web.natur.cuni.cz/~langhamr/lectures/vtfg1/mapinfo_2/barvy/colors.html)

### Sequential Sangria - Peach 

| Ramp | Alias |  Hex | RGB |
| --- | --- | --- | --- |
| SangriaPeach-L1 | $Sangria | ![\#7A0001](https://placehold.it/15/7A0001/000000?text=+) `#7A0001` | rgb(122,0,1) |
| SangriaPeach-L2 | $Tabasco | ![\#9B0001](https://placehold.it/15/af2311/000000?text=+) `#9B0001` | rgb(155,0,1) |
| SangriaPeach-L3 | $Poppy | ![\#B72715](https://placehold.it/15/B72715/000000?text=+) `#B72715` | rgb(183,39,21) |
| SangriaPeach-L4 | $Rust | ![\#D24327](https://placehold.it/15/D24327/000000?text=+) `#D24327` | rgb(210,67,39)|
| SangriaPeach-L5 | $Sockeye | ![\#EF5D3A](https://placehold.it/15/EF5D3A/000000?text=+) `#EF5D3A` | rgb(239,93,58) |
| SangriaPeach-R5| $Coral | ![\#FF7D57](https://placehold.it/15/FF7D57/000000?text=+) `#FF7D57` | rgb(255,125,87) |
| SangriaPeach-R4| $DustySalmon | ![\#FFA182](https://placehold.it/15/FFA182/000000?text=+) `#FFA182` | rgb(255,161,130) |
| SangriaPeach-R3| $DustyPink | ![\#FFC3AC](https://placehold.it/15/FFC3AC/000000?text=+) `#FFC3AC` | rgb(255,195,172) |
| SangriaPeach-R2| $SpringPeach | ![\#FFE5D8](https://placehold.it/15/FFE5D8/000000?text=+) `#FFE5D8` | rgb(255,229,216) |
| SangriaPeach-R1| $Peach | ![\#FEF5F0](https://placehold.it/15/FEF5F0/000000?text=+) `#FEF5F0` | rgb(254,245,240) |

```
'#7A0001','#9B0001','#B72715','#D24327','#EF5D3A','#FF7D57','#FFA182','#FFC3AC','#FFC3AC','#FFE5D8', '#FEF5F0'
```

```d3.scale.threshold()
.range(['#7A0001','#9B0001','#B72715','#D24327','#EF5D3A','#FF7D57','#FFA182','#FFC3AC','#FFC3AC','#FFE5D8', '#FEF5F0']);
```

---

### Sequential Money - Foam

| Ramp | Alias | Hex | RGB |
| --- | --- | --- | --- |
| $MoneyFoam-L1 | $Money | ![\#9b0001](https://placehold.it/15/46825a/000000?text=+) `#46825a` | rgb(70,130,90) |
| $MoneyFoam-L2 | $Bills | ![\#578e69](https://placehold.it/15/578e69/000000?text=+) `#578e69` | rgb(87,142,105) |
| $MoneyFoam-L3 | $SpringLeaves | ![\#699c79](https://placehold.it/15/699c79/000000?text=+) `#699c79` | rgb(105,156,121) |
| $MoneyFoam-L4 | $NewMoss | ![\#79a887](https://placehold.it/15/79a887/000000?text=+) `#79a887` | rgb(118,165,132) |
| $MoneyFoam-L5 | $BayLeaf | ![\#8bb597](https://placehold.it/15/8bb597/000000?text=+) `#8bb597` | rgb(139,181,151) |
| $MoneyFoam-R5 | $Summer | ![\#9cc2a7](https://placehold.it/15/9cc2a7/000000?text=+) `#9cc2a7` | rgb(156,194,167) |
| $MoneyFoam-R4 | $Oregano | ![\#aecfb8](https://placehold.it/15/aecfb8/000000?text=+) `#aecfb8` | rgb(174,207,184) |
| $MoneyFoam-R3 | $Thyme| ![\#c0dcc9](https://placehold.it/15/c0dcc9/000000?text=+) `#c0dcc9` | rgb(192,220,201) |
| $MoneyFoam-R2 | $DustySeafoam | ![\#d2e9da](https://placehold.it/15/d2e9da/000000?text=+) `#d2e9da` | rgb(210,233,218) |
| $MoneyFoam-R1 | $Seafoam | ![\#e4f7eb](https://placehold.it/15/e4f7eb/000000?text=+) `#e4f7eb` | rgb(228,247,235) |

```
'#46825a','#578e69','#699c79','#79a887','#8bb597','#9cc2a7','#aecfb8','#c0dcc9','#d2e9da','#e4f7eb'

```

```
d3.scale.threshold()    .range(['#46825a','#578e69','#699c79','#79a887','#8bb597','#9cc2a7','#aecfb8','#c0dcc9','#d2e9da','#e4f7eb']);
```

---

### Sequential Yellow-Red

| Ramp | Alias | Hex | RGB |
| --- | --- | --- | --- |
| $YellowRed-L1 | $Yellow | ![\#ffe37e](https://placehold.it/15/ffe37e/000000?text=+) `#ffe37e` | rgb(255,227,126) |
| $YellowRed-L2 | $Gold | ![\#ffd272](https://placehold.it/15/ffd272/000000?text=+) `#ffd272` | rgb(255,210,114) |
| $YellowRed-L3 | $OrangeGold | ![\#fec166](https://placehold.it/15/fec166/000000?text=+) `#fec166` | rgb(254,193,102) |
| $YellowRed-L4 | $Orange3 | ![\#fcaf5a](https://placehold.it/15/fcaf5a/000000?text=+) `#fcaf5a` | rgb(252,175,90) |
| $YellowRed-L5 | $Orange2 | ![\#f99e4e](https://placehold.it/15/f99e4e/000000?text=+) `#f99e4e` | rgb(249,158,78) |
| $YellowRed-R5 | $Orange | ![\#f68c43](https://placehold.it/15/f68c43/000000?text=+) `#f68c43` | rgb(246,140,67)) |
| $YellowRed-R4 | $Apricot3 | ![\#f37937](https://placehold.it/15/f37937/000000?text=+) `#f37937` | rgb(243,121,55) |
| $YellowRed-R3 | $Apricot2| ![\#EF662C](https://placehold.it/15/EF662C/000000?text=+) `#EF662C` | rgb(239,102,44) |
| $YellowRed-R2 | $Apricot | ![\#ea5021](https://placehold.it/15/ea5021/000000?text=+) `#ea5021` | rgb(234,80,33) |
| $YellowRed-R1 | $GOP | ![\#e53516](https://placehold.it/15/e53516/000000?text=+) `#e53516` | rgb(229,53,22) |

```
'#ffe37e','#ffd272','#fec166','#fcaf5a','#f99e4e','#f68c43','#f37937','#ef662c','#ea5021','#e53516'

```

```
d3.scale.threshold()
    .range(['#ffe37e','#ffd272','#fec166','#fcaf5a','#f99e4e','#f68c43','#f37937','#ef662c','#ea5021','#e53516']);
```

---
