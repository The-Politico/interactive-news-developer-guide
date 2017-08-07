### Sections
Encasing chunks of a story in [section](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Using_HTML_sections_and_outlines) tags will give them the proper padding in the story well. Simply wrap the section of the story in `<section></section>` tags and watch it work.

If you want your section to fit the story well, ad the class `content-fit`, otherwise it will span the whole well. `max-width` will make the section span 800px per the rules on aligning content above.

```html
<section class="content-fit">
<h2>Section header</h2>
<p>I'll have the correct padding now.</p>
</section>

<section class="content-fit">
<h2>Another section header</h2>
<p>Me too!</p>
</section>

```







