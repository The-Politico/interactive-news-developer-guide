# Parenthetical

Need to toss to another story? Here's a Politico.com style refer you can use in your story.

---

![](/assets/parethetical.png)

```html
<div class="refer row content-fit">
<a target="blank" href="###">
    <div class="col-xs-3">
      <figure>
      <img src="http://static.politico.com/dims4/default/a900938/2147483647/legacy_thumbnail/90x49%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2F49%2Fdf%2F50c5d1664bccad27cfdb57f610f9%2F170728-pryan-mccarthy-mcmorris-getty-1160.jpg" />
    </figure>
    </div>
    <div class="col-xs-9">
      <h5>Section title</h5>
      <h4>Headline of the link you are referring to</h4>
      <p> By <span class="bold uppercase">First Last</span> and <span class="bold uppercase">First Last</span></p>
    </div>
</a>
</div>
```

So you want to stack a few of them at the bottom of a story.   
We got you

* adds the read more h4, also an `<hr>` between refer items

![](/assets/stacked-refer.png)

```html
<h4 class="content-fit refer-toss">Read More</h4>
<div class="refer stacked row content-fit">

<a target="blank" href="http://www.politico.com/story/2017/10/13/trump-opposes-bipartisan-obamacare-rescue-plan-243752">
    <div class="col-xs-3">
      <figure>
      <img src="https://static.politico.com/dims4/default/78007bb/2147483647/legacy_thumbnail/403x218%3E/quality/90/?url=http%3A%2F%2Fstatic.politico.com%2F21%2Fdf%2Fd3a102d5412bb9fc6a0aa8bc300c%2F22-donald-trump-104-ap-1160.jpg" />
    </figure>
    </div>
    <div class="col-xs-9">
      <h5>Health care</h5>
      <h4>Trump opposes bipartisan Obamacare rescue plan</h4>
      <p> By <span class="bold uppercase"> BURGESS EVERETT,</span> <span class="bold uppercase">Racheal Bade</span> and <span class="bold uppercase"> Josh Dawsey</span></p>
    </div>
</a>

<hr>

<a target="blank" href="http://www.politico.com/story/2017/10/13/trump-opposes-bipartisan-obamacare-rescue-plan-243752">
    <div class="col-xs-3">
      <figure>
      <img src="https://static.politico.com/dims4/default/ec13504/2147483647/legacy_thumbnail/403x218%3E/quality/90/format/jpg/?url=http%3A%2F%2Fstatic.politico.com%2Fa8%2F3d%2Ff25384ab40bd816b1069dc6fdeed%2Fgiphy-1.gif" />
    </figure>
    </div>
    <div class="col-xs-9">
      <h5>Health care</h5>
      <h4>9 ways Trump is undercutting Obamacare without Congress</h4>
      <p> By <span class="bold uppercase"> Jason Millman</p>
    </div>
</a>
</div>
```



