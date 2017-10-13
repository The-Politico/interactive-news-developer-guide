# Sections

Are a great way to break your storytelling into digestible bites chunks

---

### What is it?

> The [section](http://w3c.github.io/html/sections.html#elementdef-section) element [represents](http://w3c.github.io/html/dom.html#represent) a generic section of a document or application. A section, in this context, is a thematic grouping of content. Each`section`should be identified, typically by including a heading

#### 

### **Why we like them**

`Sections` add en extra bit of hierarchy to your build by offsetting thematic content with white space. They also allow you to target sections of content with a over-arching class.

To align your section to the paragraph text append `.content-fit`. For sections you want to span **larger** than the well, experiment with appending a class of `large` or `extra-large`to your section, which expand the well to 800px and 1200px respectively.  Without a defined width, your section will default to the full width of the page.

#### 

### **When to use them**

Sometimes you need an extra bit of separation for a visual element, like a card-stack, or graphic. Or maybe it's a pause between ideas, that needs more than the hierarchy you can obtain from typography alone.  Wrapping this chunk in a section will give the idea breathing room and help distinguish it from preceding and subsequent content.

```html
<section class="content-fit uno">
    <h2>I am header in a section</h2>
    <p>I'll have the correct padding now.</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>
</section>

<section class="content-fit segundo">
    <h2>I am header in a section</h2>
    <p>I'll have the correct padding now.</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>

    <h2>I am a header in a section</h2>
    <p>Me too!</p>
</section>
```

#### 

### **When you probably don't need them**

Our H2 and H3 groups are smart enough to be used solo. If you have more than one group of h2s or h3s \(like in the example above\), you might consider wrapping them in a section.

![](/assets/not-needed-section.png)

