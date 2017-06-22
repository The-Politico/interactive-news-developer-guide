## Election

| Name | Hex | RGB |
| --- | --- | --- |
| $DemBlue | ![\#114ca1](https://placehold.it/15/114ca1/000000?text=+) `#114ca1` | rgb\(17,76,161\) |
| $GOPRed | ![\#dc2700](https://placehold.it/15/dc2700/000000?text=+) `#dc2700` | rgb\(220,39,0\) |

---

### Demp Ramp

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $DemBlue | ![\#114ca1](https://placehold.it/15/114ca1/000000?text=+) `#114ca1` | rgb\(17,76,161\) |
| $DemBlue2 | ![\#4561ac](https://placehold.it/15/4561ac/000000?text=+) `#4561ac` | rgb\(69,97,172\) |
| $DemBlue3 | ![\#6676b8](https://placehold.it/15/6676b8/000000?text=+) `#6676b8` | rgb\(102,118,184\) |
| $DemBlue4 | ![\#838dc3](https://placehold.it/15/838dc3/000000?text=+) `#838dc3` | rgb\(131,141,195\) |
| $DemBlue5 | ![\#9ea5ce](https://placehold.it/15/9ea5ce/000000?text=+) `#9ea5ce` | rgb\(158,165,206\) |
| $DemBlue6 | ![\#b9bdd9](https://placehold.it/15/b9bdd9/000000?text=+) `#b9bdd9` | rgb\(185,189,217\) |
| $DemBlue7 | ![\#d4d6e4](https://placehold.it/15/d4d6e4/000000?text=+) `#d4d6e4` | rgb\(212,214,228\) |

---

### GOP Ramp

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $GOPRed | ![\#dc2700](https://placehold.it/15/dc2700/000000?text=+) `#dc2700` | rgb\(220,39,0\) |
| $GOPRed2 | ![\#E64F29](https://placehold.it/15/E64F29/000000?text=+) `#E64F29` | rgb\(230,79,41\)\) |
| $GOPRed3 | ![\#ed6d49](https://placehold.it/15/ed6d49/000000?text=+) `#ed6d49` | rgb\(237,109,73\) |
| $GOPRed4 | ![\#f38869](https://placehold.it/15/f38869/000000?text=+) `#f38869` | rgb\(243,136,105\) |
| $GOPRed5 | ![\#f6a289](https://placehold.it/15/f6a289/000000?text=+) `#f6a289` | rgb\(246,162,137\) |
| $GOPRed6 | ![\#f7bcaa](https://placehold.it/15/f7bcaa/000000?text=+) `#f7bcaa` | rgb\(247,188,170\) |
| $GOPRed7 | ![\#f5d6cc](https://placehold.it/15/f5d6cc/000000?text=+) `#f5d6cc` | rgb\(245,214,204\) |

---

### Diverging

![](/assets/golden_magenta.png)

| Dem Ramp | Hex | RGB |
| --- | --- | --- |
| $Goldenrod | ![\#ffa602](https://placehold.it/15/ffa602/000000?text=+) `#ffa602` | rgb\(255,166,2\) |
| $DarkMagenta | ![\#810082](https://placehold.it/15/810082/000000?text=+) `#810082` | rgb\(129,0,130\) |

```html
#ffa602 #f3962c #e6863e #d9764c #cc6657 #bf5561 #b1446a #a23472 #92207a #810082
```

```html
'#ffa602','#f3962c','#e6863e','#d9764c','#cc6657','#bf5561','#b1446a','#a23472','#92207a','#810082'
```

```html
d3.scale.threshold()
    .range(['#ffa602','#f3962c','#e6863e','#d9764c','#cc6657','#bf5561','#b1446a','#a23472','#92207a','#810082']);
```

```
function palette(min, max) {
    var d = (max-min)/10;
    return d3.scale.threshold()
        .range(['#ffa602','#f3962c','#e6863e','#d9764c','#cc6657','#bf5561','#b1446a','#a23472','#92207a','#810082'])
        .domain([min+1*d,min+2*d,min+3*d,min+4*d,min+5*d,min+6*d,min+7*d,min+8*d,min+9*d,min+10*d]);
}
```



