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

### Sections
Adding a section class will give sections the proper padding in the story well. 
Simply wrap the section of the story in `<section></section>` tags and watch it work.

Currently sections are locked to 600px, we'll be updating this shortly to follow the alignment rules below.

```css
section{
  margin: 0 auto;
  max-width: 600px;
  padding: 1.5em 0;
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



