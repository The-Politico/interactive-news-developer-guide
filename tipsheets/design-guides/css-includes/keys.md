# Keys

So, you wanna make a key.

---

Easy.

Color swatches are set by the class placed on the `span`. You'll need to write a rule for the `background-color` in your `_key.scss` file.

![](/assets/key-duo.png)

### **The html**

```html
  <div class="key clearfix">
      <span class="dem"></span>Dem
      <span class="gop"></span>GOP
      <!-- <span class="teal"></span>Other -->
  </div>
```

### **Css example:**

```css
span{
    display: inline-block;
    width: 10px;
    height: 10px;
    border-radius: 2px;
    margin: 0 2px 0 5px;

    &:first-of-type{
      margin-left: 0;
    }

    &.dem{
      background-color: $dem;
    }
    &.gop{
      background-color: $gop;
    }
    &.teal{
      background-color: $teal;
    }
  }
```



### **What it looks like in action** ![](/assets/key-left.png)



