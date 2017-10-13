# Cards

Cards are a great way to group data or call out key points.

Some early prototypes here: [Is Obamacare dead yet?](http://www.politico.com/interactives/2017/senate-obamacare-repeal-vote-results-count/) , [How past income tax rate cuts on the wealthy affected the economy](https://www.politico.com/interactives/2017/gop-tax-rate-cut-wealthy/) and  [Reconciliation Explained](http://www.politico.com/interactives/2017/what-is-reconciliation/)

---

Default card background renders gray and mirrors `.sans.small` style

```html
<div class="card">
        <h2>Card Title</h2>
        <h6>Subtitle if needed</h6>
        <p>Paragraph text</p>
</div>
```

![](/assets/default-card.png)

### But! We have other styles available too!

**Border Bottom**

```html
        <h2 class="border-bottom">Card Title</h2>
        <h6>Subtitle if needed</h6>
        <p>You can see the border-bottom style on the h2 here. Does what you would expect</p>

        <h6>Subtitle if needed</h6>
        <p>A variation of the ordinary lorem ipsum text has been used in typesetting.</p>
</div>
```

![](/assets/card-border-bottom.png)

### 

### **Serif header and body type**

```html
        <h2>Card Title</h2>
        <p>Look up! A serif style is appended to the card</p>

        <p>Does what you'd expect here too.</p>
</div>
```

![](/assets/serif-card.png)





### **Color-coded cards**

The border-bottom and H2 is set to default to $gop red. You can override this in the css, but writing appending a class like .dem, in this example.

```html
        <h2>Card Title</h2>
        <h6>Subtitle if needed</h6>
        <p>A variation of the ordinary lorem ipsum text has been used.</p>
</div>

<div class="card color-coded">
        <h2>Card Title</h2>
        <h6>Subtitle if needed</h6>
        <p>By advertisements for Letraset transfer sheets or earlier.</p>
</div>
```

![](/assets/color-coded-cards.png)

