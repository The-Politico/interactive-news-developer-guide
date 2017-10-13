# Lists

Here are some quick style options for lists

---

Here is a list with `small`, `sans`, `no-indent` and `border` class applied to the `ul` level

![](/assets/list-border.png)

this one has no `border` applied

![](/assets/list-no-border.png)

```html
<section class="small sans content-fit">
<h3 class="text-align-left">Links to css hacks</h3>
<ul class="no-bullets no-indent border">
  <li>
    <a target="blank" href="https://politico.gitbooks.io/politico-newsroom-developer-guide/content/tipsheets/handy-css-tricks/text-styles.html">Controlling content widths + Text styles, small type too</a>
  </li>

  <li>
    <a target="blank" href="https://politico.gitbooks.io/politico-newsroom-developer-guide/content/tipsheets/handy-css-tricks/text-alignment.html">How to align text</a>
  </li>

  <li>
    <a target="blank" href="https://politico.gitbooks.io/politico-newsroom-developer-guide/content/tipsheets/design-guides/css-includes/cards.html">Different card styles</a>
  </li>

  <li>
    <a target="blank" href="https://politico.gitbooks.io/politico-newsroom-developer-guide/content/tipsheets/handy-css-tricks/sections.html">When to use a section</a>
  </li>

</ul>
</section>
```

```css
ul.no-bullets{
  li{
    list-style: none;
  }
  &.no-indent{
        -webkit-margin-before: 0;
        -webkit-padding-start: 0px;
  }
  &.border{
    li{
    border-top: 1px solid #ddd;
    padding: 10px 0;
    }
  }
}
```



