# PHOTOS

Where to access photos: AP [Website](http://www.apimages.com/)  \|   Getty [Website](http://www.gettyimages.com/)

---

### Images
All images should be wrapped in a figure. All photos should run with a credit. If the photographer is anonymous you may credit only the photo service ie: Getty Images or AP Photo

```html
<figure>
    <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
    <figcaption class="figcaption">
        Caption text here. <figcredit> | John Shinkle/POLITICO </figcredit>
    </figcaption>
</figure>

```


### Full span image at all breakpoints

```html
</article>
<!-- You must close the article to go full span, and then reopen it. -->
<figure>
   <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
    <figcaption class="figcaption">
        Caption text here. 
        <figcredit> | John Shinkle/POLITICO </figcredit>
    </figcaption>
</figure>

<article class="container">
```

### No gutters on the phone

```html
<figure class="no-gutters-phone">
    <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
    <figcaption class="figcaption">
        Caption text here. 
        <figcredit> | John Shinkle/POLITICO </figcredit>
    </figcaption>
</figure>
```

### Diptych

```html
<div class="diptych">
    <figure>
        <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
        <figcaption class="figcaption">
            Caption text here. 
            <figcredit> | John Shinkle/POLITICO </figcredit>
        </figcaption>
    </figure>

    <figure>
        <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
        <figcaption class="figcaption">
            Caption text here. 
            <figcredit> | John Shinkle/POLITICO </figcredit>
        </figcaption>
    </figure>
    <div class="clear"></div>
</div>
```

### Triptych

```html
<div class="triptych">
      <figure>
        <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
        <figcaption class="figcaption">
            Caption text here. 
            <figcredit> | John Shinkle/POLITICO </figcredit>
        </figcaption>
    </figure>

      <figure>
        <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
        <figcaption class="figcaption">
            Caption text here. 
            <figcredit> | John Shinkle/POLITICO </figcredit>
        </figcaption>
    </figure>

    <figure>
        <img src="https://static.politico.com/dims4/default/00bb1f8/2147483647/resize/1160x%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2Fe6%2F99%2Fcd6aa5bc43dcb92588f25d90f16d%2Fgoldsmith-photogallery-13.jpg" />
        <figcaption class="figcaption">
            Caption text here. 
            <figcredit> | John Shinkle/POLITICO </figcredit>
        </figcaption>
    </figure>

<div class="clear"></div>
</div>
```



