### Text alignment

```css
.center-align-text{
  text-align: center;
}

.left-align-text{
  text-align: left;
}

.right-align-text{
  text-align: right;
}
```


### Aligning content to the main well

```css
.content-fit{
  max-width: 600px;
  @include margin-auto;
}

.large{
  max-width: 800px;
  @include margin-auto;
}

.full-width{
  width: 100%;
  @include margin-auto;
}
```


### Sections
Encasing chunks of a story in [section](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using_HTML_sections_and_outlines) tags will give them the proper padding in the story well. Simply wrap the section of the story in `<section></section>` tags and watch it work.

If you want your section to fit the story well, ad the class `.content-fit`

```html
<section>
<h2>Section header</h2>
<p>I'll have the correct padding now.</p>
</section>

<section>
<h2>Another section header</h2>
<p>Me too!</p>
</section>


```




