# Aligning text and content wells

## Text alignment

```css
.text-align-center{
  text-align: center;
}

.text-align-center{
  text-align: left;
}

.text-align-center{
  text-align: right;
}
```

## Aligning content to the main well

```css
.content-small{
  max-width: 400px;
  @include margin-auto;
}

.content-fit{
max-width: 550px;
@include margin-auto;
}

.content-large{
max-width: 800px;
@include margin-auto;
}

.content-extra-large{
max-width: 1200px;
@include margin-auto;
}

.content-full-width{
width: 100%;
@include margin-auto;
}
```

