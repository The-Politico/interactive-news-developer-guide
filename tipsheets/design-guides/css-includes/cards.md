# Cards

Cards are a great way to group data or call out key points.

Some early prototypes here: [Is Obamacare dead yet?](http://www.politico.com/interactives/2017/senate-obamacare-repeal-vote-results-count/) , [How past income tax rate cuts on the wealthy affected the economy](https://www.politico.com/interactives/2017/gop-tax-rate-cut-wealthy/) and  [Reconciliation Explained](http://www.politico.com/interactives/2017/what-is-reconciliation/)

---

Default card background renders gray and mirrors `.sans.small` style

Want to grab three cards already formatted in a row and section? Scroll down to the bottom of this page 🎁 

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
<div class="card">
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
<div class="card serif">
        <h2>Card Title</h2>
        <p>Look up! A serif style is appended to the card</p>

        <p>Does what you'd expect here too.</p>
</div>
```

![](/assets/serif-card.png)





### **Color-coded cards**

The border-bottom and H2 is set to default to $gop red. You can override this in the css, but writing appending a class like .dem, in this example.

```html
<section>
  <div class="row">
    <div class="col-sm-4">
    
      <div class="card color-coded dem">
        <h2>Card Title</h2>
        <p>A variation of the <span class="highlight">ordinary lorem</span> ipsum <span class="highlight">advertisements</span> for Letraset transfer sheets.</p>
      </div>
    </div>
    
    <div class="col-sm-4">
      <div class="card color-coded gop">
        <h2>Card Title</h2>
        <p>You can see the border-bottom style on the h2 here. Does what you would expect</p>
      </div>
    </div>

    <div class="col-sm-4">
      <div class="card color-coded teal">
        <h2>Card Title</h2>
        <p>Look up! Appended to the card</p>
      </div>
    </div>
    
  </row>
</section>
```

![](/assets/color-coded-cards.png)

