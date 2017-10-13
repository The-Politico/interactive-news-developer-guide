### Text transformations + highlight style

Sans, serif, bold, uppercase, and even .small styles for paragraph text. Let's do it.

---

```css
.sans{
  font-family: $proxima;
}

.serif{
  font-family: $tisa;
}

.bold{
  font-weight: 700;
}

.unbold{
font-weight: 500;
}

.italic{
text-style: italic;
}

.uppercase{
  text-transform: uppercase;
}

.highlight {
    background-color: #fff7a5;
    box-shadow: 0.2rem 0 0 #fff7a5, -0.2rem 0 0 #fff7a5;
    margin: auto 2px;
}
```



### **Highlight for em-PHA-sis**

Our style is to **include punctuation**, commas or periods etc. inside the span class.

```html
of his generals; <span class="highlight">preservation and command</span> of the army
```

![](/assets/highlighter.png)

### 

### **Small Paragraph text option - serif + sans**

Our cards default to this, but you may want to use it in other places. Here's how.

```html
<p class="small">This is what small paragraph text looks like.</p>
<p class="small sans">This is what small sans paragraph text looks like</p>
```

**In action**

![](/assets/smally.png)

